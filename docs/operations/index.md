# Introduction to Operations

The following documentation is meant to give you an idea and examples of implementations in Kenya. These documents can act as general templates for how to setup a Community Inclusion Currency.

## Voucher (CIC) Creation

Our [Community Training Guide](/operations/training/) gives a basic training for identifying local resources and sharing them together using a CIC.

1. **Resource Mapping**: Working with your community to map out resources and needs. Often people don’t realize how much they can offer and how much they can support each-other. The Training guide goes through the majority of these steps. Also note that individuals and organizations like Grassroots Economics can create their own vouchers.
1. **Learning through games**: Ensure that everyone involved or expected to utilize a CIC is able to play through a demonstration with others. Work out all the kinks BEFORE you start.
1. **Demonstrate Collective Commitments**: Coming up with agreements on what each member of the community can offer to the whole in exchange for vouchers.
1. **Audits, Endorsements and Conflict Mitigation**: Commitments should be internally audited by the community and as well with a designated auditor to ensure that the vouchers can be redeemed in a  reasonable amount of time. A mediator should be assigned to deal with conflicts, like when a member spends but refuses to redeem vouchers they created.
1. **Agreements Signed (see [legal section](/legal/) )**
    1. **Clearing Union Implementation**: The above work defining the Voucher is collected into a Clearing Union Implementation.
    1. **Service Agreement**: Should the community need a service provider, then an agreement is developed between the community and a Platform Service Provider.
1. **Minting / Voucher Creation**: This is generally handled by a Platform Service Provider like Grassroots Economics, who will validate the groups commitments, audits and endorsements and deploy a contract on a ledger that is visible to anyone. This contract (smart contract) will hold all the relevant information about the Voucher and create the supply.
1. **Initial Voucher Distribution**: After minting, Vouchers will then be distributed to the Community that has committed to redeeming them with full transparency. This will be done as per the instructions of the community and can be facilitated by a community treasurer. It is recommended to have a voted on community fund /treasury which will also collect any levies (demurrage).
1. **Greater Community Outreach**: While the community of issuers may begin to assign and clear vouchers among each other, they will generally want to spread their usage to their greater community. They can choose to give new users a small amount out of a community fund as is done with Sarafu, or to simply try to sell the Vouchers or use them to buy goods or services.
1. **Long Term Maintenance**: Imbalance / inequality is a common character of any credit system. Some people may end up with a lot and some people may end up with zero. Having regular meetings, or market days and actively clearing imbalances together is highly recommended. A levy on accounts is a good way to ensure that people have no incentive to hold Vouchers as a form of savings or investment and that they continue to circulate as a medium of exchange.


## Technology Setup

Generally the technical setup is done by a local Platform Service Provider like Grassroots Economics. The more local the better.

1. **Open Source (CopyLeft) Software**: Ensure that you trust the software being used and that even if it is open source now, that improvements and upgrades will remain open source. Check out our [stack](/software/).
1. **Distributed Ledger**: We highly recommend developing your own ledger system where members of the community hold nodes that decentralize and secure the ledger.
1. **Interfaces / Wallets**: We’ve built custodial systems that enable users to assign guardians that can help them reset lost passwords.
1. **Data Sharing**: Given the consent of the community, anonymous transaction data can be recorded and displayed



## Humanitarian Support

1. **Stakeholder Gatherings and Training**: These are similar to the steps mentioned in Voucher creation, but will often involve a wider range of stakeholders including local government.
1. **Capacity Building**: When identifying resources that people have to share – gaps in those resources compared to need often arise. Filling these gaps through training and asset development can help the community have a solid framework for voucher redemption.
1. **Evidence based support**
    1. **Impact Indexing**: Data from CIC circulation and endorsements from validators is indexed based on Sustainable Development Goals and a rank and reward can be calculated for support
    1. **Donor Support**: Donors can be rewarded with impact data in the form of a digital certificate they can also followup on future impacts.
    1. **Treasuries**: Based on results from Indexing a Humanitarian organization can choose to purchase vouchers with donor funds (held in *Treasuries*).
    1. **Redistribution**: Based on results from Indexing CICs held in *Treasuries* can be redistributed directly to those people in need.

```graphviz dot hum_dev.svg
digraph D {
  rankdir=TB;
  subgraph cluster_v_1 {

    label = "CIC";
     style="rounded"


	chama [label= "Community Groups"]
        nd_1a   [label = "General\nMember"];
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
	datam [label= "Anonymous CIC trade \n& meta data" , shape = cylinder]


  }

  subgraph cluster_market_5 {
     rank=tb;
     label = "Impact Markets";
     style="rounded"
	cucm [label= "CIC Markets", shape = box]
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
      <tr><td align="left" port="i1"> </td><td>CICs</td></tr>
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
