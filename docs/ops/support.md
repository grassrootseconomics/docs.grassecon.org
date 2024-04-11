# Humanitarian Support

Supporters that wish to help empower communities and build strong resilient and regenerative local economies toward other goals like sustainable envirmental or educational programs, have a lot of options when working with Community Asset Vouchers CAVs.

1. **Stakeholder Gatherings and Training**: These are similar to the steps mentioned in [Voucher creation](/ops/voucher/), but will often involve a wider range of stakeholders including local government.
1. **Capacity Building**: When identifying resources that people have to share – gaps in those resources compared to local needs often arise. Filling these gaps through [training](/operations/training/) and communal asset development can help the community have a solid framework for sustainable voucher redemption.
1. **Evidence based support**
    1. **Impact Indexing**: Data from CAV circulation and endorsements from validators is indexed based on Sustainable Development Goals and a rank and reward can be calculated for support
    1. **Donor Support**: Donors can recieve impact data in the form of a digital certificate they can also followup on future impacts.
    1. **Treasuries**: Based on results from Indexing a Humanitarian organization can choose to purchase vouchers with donor funds (held in *Treasuries*).
    1. **Redistribution**: Based on results from Indexing CAVs held in *Treasuries* can be redistributed directly to those people in need.

```graphviz dot hum_dev.svg
digraph D {
  rankdir=TB;
  subgraph cluster_v_1 {

    label = "CAV";
     style="rounded"


	chama [label= "Community Groups"]
        nd_1a   [label = "General\nMember", href="https://docs.grassecon.org/commons/"];
        nd_2a   [label = "General\nMember"];
        nd_3a   [label = "General\nMember"];
        nd_4a   [label = "General\nMember"];
        chama -> nd_1a -> nd_2a -> nd_3a -> nd_4a -> chama
	nd_3a -> nd_1a

  }

  subgraph cluster_data_2 {

    label = "Impact Evidence";
     style="rounded"


	endo [label= "Endorsements"]
	datam [label= "Anonymous CAV trade \n& meta data" , shape = cylinder]


  }

  subgraph cluster_market_5 {
     rank=tb;
     label = "Impact Markets";
     style="rounded"
	cucm [label= "CAV Markets / Commitment Pools", shape = box]
	nftm [label= "Impact Data Markets", shape = box]

  }


  subgraph cluster_index_3 {

    label = "Humanitarian Supporters";
     style="rounded"


	training [label= "Training \n& Capacity Building"]
	indexer [label= "Indexing", shape = cylinder]
	treasuries [label= "Treasuries", shape = cylinder]
	donors [label= "Donors"]
	impacti [label= "Impact Investors"]

  }

  chama -> treasuries
  treasuries->chama [style = dotted];
  treasuries->training [style = dotted];
  donors -> treasuries [style = dotted];
  impacti -> treasuries [style = dotted, constraint=false];
  impacti -> nftm [style = dashed, constraint=false];
  impacti -> cucm
    treasuries -> donors [style = dashed];
  treasuries -> impacti [style = dashed];
  treasuries -> impacti

  chama -> datam [ style = dashed    ];

  endo -> datam [ style = dashed    ];
  datam -> indexer [ style = dashed    ];
  indexer -> treasuries [ style = dashed    ];

  chama -> training;
  training -> treasuries
  treasuries  -> nd_1a
  treasuries  -> nd_3a


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
      <tr><td align="left" port="i1"> </td><td>CAVs</td></tr>
      <tr><td align="left" port="i2"> </td><td>Impact Evidence/Data</td></tr>
      <tr><td align="left" port="i3"> </td><td>Fiat / other vouchers</td></tr>
      </table>>]
    key:i1 -> key2:i1
    key:i2 -> key2:i2 [ style=dashed ]
    key:i3 -> key2:i3 [ style=dotted ]
   }

   edge[ style = invis ];
   {nd_3a nftm} -> key:i1;

}
```
