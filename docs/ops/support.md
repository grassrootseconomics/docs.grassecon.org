# Humanitarian Support

Supporters seeking to empower communities and cultivate resilient, regenerative economies—whether for environmental goals, education, health, or mutual aid—have a variety of ways to engage through **Commitment Pooling**.

Commitment Pooling shifts support from charity to reciprocity—honoring local contributions and routing support through trusted commitments.

## Ways to Support

1. **Stakeholder Gatherings and Training**  
   Similar to the process described in [Voucher Creation](/ops/voucher/), initial gatherings should include local leaders, community groups, and government. These sessions introduce the Commitment Pooling model and help coordinate trust flows.

2. **Capacity Building**  
   Through resource mapping and exchange simulations, gaps between community needs and existing capacities are identified. Supporters can fill these gaps through training, toolkits, and shared assets that enhance the community’s ability to fulfill its pooled commitments.

3. **Evidence-Based Support**  
   Commitment Pooling produces traceable, anonymized data on trust, exchange, and fulfillment.

   - **Impact Indexing**  
     All voucher circulation, redemptions, and endorsements are indexed to SDGs and local goals.
   
   - **Donor Support**  
     Donors receive digital certificates of impact and may follow future flows of support.
   
   - **Treasuries**  
     Donor contributions can be converted into pool-compatible vouchers and held in community treasuries.
   
   - **Redistribution**  
     Vouchers in treasuries may be routed to vulnerable members or used to fund local commons efforts (like clean water or education initiatives).

```graphviz
digraph D {
  rankdir=TB;

  subgraph cluster_v_1 {
    label = "Commitment Pool";
    style="rounded"

    chama [label= "Community Pool"]
    nd_1a   [label = "Member A", href="https://docs.grassecon.org/commons/"];
    nd_2a   [label = "Member B"];
    nd_3a   [label = "Member C"];
    nd_4a   [label = "Member D"];
    chama -> nd_1a -> nd_2a -> nd_3a -> nd_4a -> chama
    nd_3a -> nd_1a
  }

  subgraph cluster_data_2 {
    label = "Impact Evidence";
    style="rounded"
    endo [label= "Endorsements"]
    datam [label= "Anonymized Swap & Fulfillment Data", shape = cylinder]
  }

  subgraph cluster_market_5 {
    label = "Impact Markets";
    style="rounded"
    cucm [label= "Commitment Pools / Swap Ledgers", shape = box]
    nftm [label= "Impact Data Marketplaces", shape = box]
  }

  subgraph cluster_index_3 {
    label = "Support Ecosystem";
    style="rounded"
    training [label= "Training & Capacity Building"]
    indexer [label= "Indexing Engine", shape = cylinder]
    treasuries [label= "Community Treasuries", shape = cylinder]
    donors [label= "Donors"]
    impacti [label= "Impact Investors"]
  }

  chama -> treasuries
  treasuries -> chama [style = dotted]
  treasuries -> training [style = dotted]
  donors -> treasuries [style = dotted]
  impacti -> treasuries [style = dotted, constraint=false]
  impacti -> nftm [style = dashed, constraint=false]
  impacti -> cucm
  treasuries -> donors [style = dashed]
  treasuries -> impacti
  chama -> datam [ style = dashed ]
  endo -> datam [ style = dashed ]
  datam -> indexer [ style = dashed ]
  indexer -> treasuries [ style = dashed ]
  chama -> training
  training -> treasuries
  treasuries -> nd_1a
  treasuries -> nd_3a

  subgraph cluster_Legend_5 {
    rank = sink;
    peripheries=0;
    label = "Legend";
    node [ color="white" ]
    {rank=same; key, key2}
    key [ label=<<table border="0" cellpadding="1" cellspacing="0" cellborder="0">
      <tr><td align="right" port="i1"> </td></tr>
      <tr><td align="right" port="i2"> </td></tr>
      <tr><td align="right" port="i3"> </td></tr>
    </table>> ]
    key2 [ label=<<table border="0" cellpadding="1" cellspacing="0" cellborder="0">
      <tr><td align="left" port="i1"> </td><td>Commitment Pools / Vouchers</td></tr>
      <tr><td align="left" port="i2"> </td><td>Impact Evidence / Data</td></tr>
      <tr><td align="left" port="i3"> </td><td>Fiat or External Funds</td></tr>
    </table>>]
    key:i1 -> key2:i1
    key:i2 -> key2:i2 [ style=dashed ]
    key:i3 -> key2:i3 [ style=dotted ]
  }

  edge[ style = invis ];
  {nd_3a nftm} -> key:i1;
}
```
