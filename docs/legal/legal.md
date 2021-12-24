# Introduction to Legal

The following documentation is meant to give you templates on designing legal frameworks surrounding community driven financial instruments like Community Inclusion Currencies. [Here](/legal/data_policy/) you can also look at the Data Protection Policy of Grassroots Economics Foundation.

## Legal Framework

This legal design for a Fiscal Commons utilizes the [Nondominium](https://wiki.p2pfoundation.net/Nondominium) recursive framework, where mutually defined Instruments are utilized by (General Members) who jointly oversee active stewards (Service Providers) subject to passive custodians (Guardians) with protective governance rights of arbitration and final veto.

By developing an inclusive legal Nondominium framework an open community is created that anyone can opt into and as long as the protocols are followed they can develop member to member agreements which decentralize the commons and maintaining integrity.

- The agreements Fiscal Commons can be broken into various agreements:
    *  [Clearing Union Schema (CUS)](/legal/clearing_union_schema/): A general overarching template that defines a fiscal commons which can be implemented.
    *  [Clearing Union Implemetation (PSP)](/legal/cu_sarafu/): An implementation of the CUS by a PSP which offers training, mediation, and running various micro-services, like blockchain nodes, wallets and marketplaces.
    *  [Voucher Creation](/legal/cu_group/): An example of an individual or group that wants to create a Voucher
    *  [Intermember Service Agreement](/legal/cu_intermember/): Establishes agreements between CU Members

Note that performing legal due diligence is extremely important in any country you are in. 


```graphviz dot clearing_union2.svg
digraph D {
 compound=true;
 
  subgraph cluster_p {
      
    label = "Clearing Union";
     style="rounded"


	e [label= "Guardians"]
        nd_1   [label = "General\nMember"];
        nd_2   [label = "General\nMember"];
        nd_3   [label = "General\nMember"];
        nd_4   [label = "General\nMember"];
	serve_1   [label = "Service Agreements"];
	csp   [label = "Core Service Providers"];
        nd_1 -> serve_1 -> csp
        nd_2 -> serve_1 -> csp
        nd_3 -> serve_1 -> csp
        nd_4 -> serve_1 -> csp
	serve_1 -> e;

  }
}
```

