# Introduction to Legal

The following documentation is meant to give you templates on designing legal frameworks surrounding community driven financial instruments like Community Inclusion Currencies.

This legal design for a Economic Commons utilizes the [Nondominium](https://wiki.p2pfoundation.net/Nondominium) recursive framework, where mutually defined Instruments are utilized by (General Members) who jointly oversee active stewards (Service Providers) subject to passive custodians (Guardians) with protective governance rights of arbitration and final veto.

```graphviz dot econ_commons1.svg
digraph D {
 compound=true;

  subgraph cluster_e {

    label = "Economic Commons Framework";
     style="rounded"


  subgraph cluster_p {

    label = "Economic Commons Agreement";
     style="rounded"
     edge [arrowhead=none,arrowtail=dot,style=dashed];

     e [label= "Guardians\n(Passive Custodians)"]
     nd_2   [label = "Individual Members\n(Instrument Users)"];
     nd_1   [label = "Associations of Members\n(Instrument Issuers)"];
     	serve_1   [label = "Service Agreements",shape="note"];

	csp   [label = "Platform Service Providers\n(Active Stewards)"];
        nd_1 -> serve_1 -> csp
        nd_2 -> serve_1
	serve_1 -> e [ style = invis ];

  }
    }
}
```

By developing an inclusive legal Nondominium framework an open community is created that anyone can opt into and as long as the protocols are followed they can develop member to member agreements which decentralize the commons and maintaining integrity.

- An Economic Commons can be broken into various agreements:
    * [Grassroots Economics Commons License v1 (GECL v1)](/legal/license/): A general overarching template that defines an Economic Commons and various rights and responsibilities of its Members.
    * [Grassroots Economics Commons Agreement](/legal/agreement/): The Grassroots Economics Commons Agreement is an example Economic Commons which incorporates the GECL v1 with Grassroots Economics Foundation's Sarafu Network as its Platform. Further Grassroots Economics as a Platform Service Provider declares the Sarafu Voucher redeemable as payment for various services such as training, clearing, mediation, and running various micro-services, like blockchain nodes, wallets and marketplaces.
    * [Voucher Creation](/legal/voucher/): An example of an individual or group that wants to create a Voucher within an Economic Commons
    * [Intermember Service Agreement](/legal/service/): Establishes agreements between Economic Commons Members. In this example a Voucher creating Member wishes to subscribe to the services of a Platform Service Provider.
    * [Data Policy](/legal/data_policy/): Here is an example of a data protection policy of Grassroots Economics as a Platform Service Provider.


