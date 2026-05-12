# Commons

The Commons section holds legal and governance templates for community-driven financial instruments such as Community Asset Vouchers and Commitment Pools.

Grassroots Economics uses an Economic Commons frame so communities can define rights, responsibilities, instruments, service agreements, stewardship roles, and safeguards around shared systems. The legal design draws on the [Nondominium](https://wiki.p2pfoundation.net/Nondominium) recursive framework: members define instruments together, service providers maintain active infrastructure, and guardians hold protective governance rights such as arbitration and final veto.

* [Glossary](/edu/glossary/) of terms.

```graphviz dot econ_commons1.svg
digraph D {
 compound=true;

  subgraph cluster_e {

    label = "Economic Commons Template";
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

Through this opt-in framework, individuals and associations can join a commons, issue or use instruments, and form member-to-member agreements while preserving shared integrity and accountability.

## Core agreements and licenses

* [Economic Commons Template (ECT)](/commons/template/): A general template for Economic Commons rights, responsibilities, roles, and instruments.
* [Grassroots Economics Commons Agreement](/commons/agreement/): The Grassroots Economics Commons Agreement using Sarafu Network as its platform.
* [Voucher Declaration](/commons/voucher/): A template for an individual or group creating a Community Asset Voucher.
* [Intermember Service Agreement](/commons/service/): A template for services between Economic Commons members and platform service providers.
* [PATH License](/commons/path/): The Public Awareness & Transparent Heritage license for Community Asset Vouchers.
* [SPROUT Policy](/commons/sprout/): The Stewarded Pools for Relational Obligations and Unified Trust license for Commitment Pools.
* [SPROUT Swap Loan Terms](/commons/sprout-loan-terms/): Terms for swap loans when a pool uses signed withdrawal terms.

## Policies

* [Data Policy](/commons/data_policy/): Grassroots Economics data protection and privacy policy.
* [Social Soil Privacy Policy](/commons/privacy_policy_social_soil/): Privacy policy for the Social Soil farming and village-trading game.
* [Child Protection Policy](/commons/child_policy/): Safeguarding policy for work involving children and young people.

For a single policy index, see [Policies](/policies/).

