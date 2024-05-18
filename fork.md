This report contains 22 clusters, and largely exceeds the body maximum character size for issues. Later clusters and descriptions will be deported to an external repository that will remain un-edited after the submission of that report.

Please note that all cluster of that report are independent and have their very own description & argumentation. An issue per cluster would be a better option, but it is impossible as that many opened issues would result in my account being flagged for spam by Github.

Please treat the clusters independently and excuse those changes the size of my report forced.

# Detailed Methodology & Walkthrough

After gathering as much CEX (Binance, Coinbase, Kucoin, Bybit, OKX) Hot Wallets & Gas suppliers as possible using explorers, a simple Dune SQL request gathered about 2M5 CEX deposit addresses (the address a user sends assets to in order to deposit into a CEX) were collected.

With Dune Dashboard once again, I filtered the CEX deposit addresses that received funds from at least 7 addresses that interacted with Layer Zero regularly (using an unofficial Dune Dashboard). 

Those 7-300 sized clusters of active L0 addresses that share the same CEX deposit address were used by a script to form bigger clusters using addresses that interacted with the addresses of the cluster but not with the CEX deposit address. To limit false positive, an address had to be directly linked to at least 4 other addresses of the cluster to join the cluster. Final clusters of less than 20 addresses (21 with the CEX deposit address) were discarded.

That is the first layer of detection/proof. Every cluster has a big chunk of addresses that share the same CEX deposit address, and the addresses are linked to at least 4 other addresses of the cluster. This layer is fully automated with scripts and has, even though it's less that regular clusters due to the multiple interactions & the common CEX deposit address, a percentage of false positive addresses.

This is where the second layer of detection/proof comes in handy. For every cluster in this report, every addresses has been scanned **manually**, the false positive evicted and on-chain arguments added to the description of the cluster. Those on-chain arguments are the second layer of detection/proof and varied: the addresses of the cluster executing the same transaction at the same time with the same amounts, a similar pattern of transaction for L0 activities etc... Plenty ressources were used, like LayerZero Scan, Dune, Debank, Arkham, Etherscan and else.

This second layer done 100% manually, even though it is not time efficient, is a way to ensure the sybil nature of the clusters and limit the number of false positive. It's also a way to demonstrate work has been done & the report is not simply a dump of a huge list of addresses.

The combination of the two layers, the cluster, the usage of the same CEX deposit address for a big part of the cluster & the similar on-chain activited manually reported makes for a good detection with as little false positive as possible.

Activity predated of the Snapshot was screened over 14 blockchains: Ethereum endblock 19757726, Optimism endblock 119326917, BSC endblock 38236464, Polygon endblock 56379454, Arbi endblock 205653169, Gnosis endblock 33677943, Linea endblock 4059728, Scroll endblock 5184468, Zksync endblock 32656745, Moonbeam endblock 6045324, Moonriver endblock 6637617, FTM endblock 80127182, Base endblock 13709885, Celo endblock 25273962.

Lastly, please note links on Arkham diagrams in this report are often missing. Arkham only supports 7 out of those 14 blockchains. 

# Reward Address (If Eligible)


0xEb8006791807CFD378cF33F676E8C9c3f7d4739F

This is a fresh address.


# Table of Contents

<details>

1. [Cluster 1](#cluster-1)
2. [Cluster 2](#cluster-2)
3. [Cluster 3](#cluster-3)
4. [Cluster 4](#cluster-4)
5. [Cluster 5](#cluster-5)
6. [Cluster 6](#cluster-6)
7. [Cluster 7](#cluster-7)
8. [Cluster 8](#cluster-8)
9. [Cluster 9](#cluster-9)
10. [Cluster 10](#cluster-10)
11. [Cluster 11](#cluster-11)
12. [Cluster 12](#cluster-12)
13. [Cluster 13](#cluster-13)
14. [Cluster 14](#cluster-14)
15. [Cluster 15](#cluster-15)
16. [Cluster 16](#cluster-16)
17. [Cluster 17](#cluster-17)
18. [Cluster 18](#cluster-18)
19. [Cluster 19](#cluster-19)
20. [Cluster 20](#cluster-20)
21. [Cluster 21](#cluster-21)
22. [Cluster 22](#cluster-22)

</details>


As the cluster are independant and a description comes with every cluster, the two following sections have been regrouped.

This following section is an rotation of the list of the addresses of the cluster and its description: the CEX deposit address some of the addresses share, an Arkham diagram & the second layer of detection.



# Reported Addresses & Description







## CLUSTER 1


The first 14 addresses of the cluster share the same Binance deposit address 0xD6e68D8BD25FD515714BC934bE0D29051783bd5C. The rest are linked to numerous addresses of the cluster, multiple times.


```
0xda6609637505074cc84f5b760dfdf6232277f499
0xc82edf738dc2179d02b577b641e45bdbd686602d
0x8121d1f92681f3b7859bd2107da4be421f81d1aa
0xe08ecf1d2c5210f47585ab3609f05274e90e23c6
0x391f2661f1a11c4c6d5dc39aced59b55755f7e90
0x69cbe5511035e56ecf75ed64bd9cfc2cb21f76f3
0x2df824b39c87d971ad8d166f3eb7efc14f4f614d
0xb82eb0b4ab2df34bb948df3d90d8ea00c665ad6b
0x08b8fd3a2146c99c01dc479ab9d35667b1356fb6
0xd09381ce893219cabc0ada4d1c6692ccb7df208c
0x0b60028e4c5792057a2ef197d74726bc4bf634da
0x21b78cd0bf06b1cb2779e616808e9038eca7a22e
0xfe09eb7f49853c56ee4ce8984ec91a7a56c63076
0x235f8D840d656A0B383b4cf1fD61e1cEb5508e41
0xD6e68D8BD25FD515714BC934bE0D29051783bd5C
0xac4029ffc2795a1f39becef58ee8ce3dc0a6083c
0x4d1c90e0c8370127bf477436ba81d74dc40433a5
0x42a51ccad7885762b9376c29648d927b7e967103
0x0934f8454f857175b1e0ebc7779fccf829a99998
0x2ff3d7f7fe8a607af688616ab1675d7a8d9d4d27
0x6b83d60dba5f5e39a962b537e8691751e8e852ae
0x7d1b0df6868033e33455336e9bac32cf8e3f7b75
0x7cda487a42924b8b17d7409a2bb1b8b2cc22d5ac
0x1eb93d6d82010573f96fa59eff11a1e4fec11eac
0x4dc57171b9e4b5519a5b8276db206f8c259fac46
0x03c2ca31809be1c754e7444b3273f6bfc7144606
0xf7d111f3c68cd3ee71c980fa800044a2d8414c83
0x16812d83987aeae684242d4f93ad54086ff91277
0xdd48d65f92c9bb9572b31a2cdfd9820b00d9ee74
0xb4d1cccf8b957903aff8b353f2603a9f9465b3b9
0xc11a699bf436feaf3b9aae9a5f1d446c5cd65b83
0x688904c1cdd3589f1786a70cf546166c71930f98
0x89390c78609adc9801254a5a31671a98d4b7decb
0xa521380673e3743fe91a125c04482b50d900063f
0x99bd7219a271e73343d7c20e3bcbaeab7a3f93fe
0x10aacb34361a0cc960f34cb8c81458337be2043b
0xae52697be69e3b2f6602d7612910bfb284c16688
0x4b2a1c74712be0021f7ff68279c97ebda3b6fd19
0x5f7dbdfb223f21511fca3ccb6606fb99265708b8
0xeb2f5869082f2862f3b7e34bd269ed0b99a2b32f
0x2a25f6c27ec5331b6dfb3c6d4a8c57cf3eedc185
0x3cee3299027287ca6593813cee18e2285e2e2f40
0xc4e9e849fcbd076fbb82fa76af7ff8695b0ad172
0x768751ceab2da8db0c7cd1cb8ffe9af592c48645
0xf4964b273b3b564f05192c1c981a96b0c97cddea
0x2ee96239818e0249a70062b99e4a820bc93055cd
```





![image](https://github.com/ultratwo/sybilled20/assets/160050412/6a5637eb-c199-42de-afe2-1fac4bf038dc)


The addresses all have the same on-chain activity. For example, their latest L0 interaction is the same, the same dapps at the same time in the same order: Stargate 8-9 days ago, Holograph 21-22 days ago, Open Name 4 months ago, Stargate 8 months ago.

<details>

  ![image](https://github.com/ultratwo/sybilled20/assets/160050412/6733606c-4c91-4c13-b00e-9f4396bfe6c6)


![image](https://github.com/ultratwo/sybilled20/assets/160050412/f9dad199-aefa-4efe-ab79-badf803c699a)


![image](https://github.com/ultratwo/sybilled20/assets/160050412/be9f2aaa-8f87-4bd6-8b88-c54266513aaf)


![image](https://github.com/ultratwo/sybilled20/assets/160050412/6ab202b9-31a7-4738-acc2-44a872e8074f)

![image](https://github.com/ultratwo/sybilled20/assets/160050412/8e54ced5-b155-462e-9ae5-1ef2ccf728b4)


![image](https://github.com/ultratwo/sybilled20/assets/160050412/1f2bf0dc-546a-4b84-9196-159ecad0fb7e)


![image](https://github.com/ultratwo/sybilled20/assets/160050412/4d553763-24ce-41a9-9bca-664ec71eef93)


![image](https://github.com/ultratwo/sybilled20/assets/160050412/362012b8-cb3a-4826-b097-b7ce2cb7cbb9)

  ![image](https://github.com/ultratwo/sybilled20/assets/160050412/071b9948-74fc-4802-82f1-9cf174c9dc18)

etc...

</details>

The addresses also all have similar ENS.

The address share the same CEX deposit address, are part of a cluster with multiple links between one another, and have the same on-chain activity. This is a big scale sybil operation, probably the result of scripts.



## CLUSTER 2

The first 20 addresses of the cluster share the same Binance deposit address 0x60235Dd2DF70BDe946e58C4d2d36F24A8849fF86. 10 addresses of the cluster also use the Binance deposit address 0x6b26a065FdaF9225B79315b1131D5821Ed808051. The rest are linked to numerous addresses of the cluster, multiple times.


```
0x1f340889daaa0f62cc434ce3d2029adaa1ca1749
0xab8798b8471917659cd8c6575e894866d3c6fd2b
0x3cf2af12d37743fc081895faa5868864cb7d4b58
0xe64b63c94146f9fcf3157bff930affbd102710bd
0xb7a5c4bbcebd0ab96c0a47685fffa0b9dc7a3694
0xa31878149afaa3f700aa55d2acdd994c2d82c8cf
0x8e774fe528acf2104aa791c77bba98ad25dd1863
0x850718163d2bf34ce2352f43dd5b9e4eddaa1a21
0x1064af8a3354ad8428ef56ea66ff5aa9292b41eb
0x754e1c14619f4e0526b5559c074f07b7e89077a4
0x6aa94b563888f760f351b429ef45a53c15458572
0xe7586b22216c3d90f8f28ba36afb57c66a02a981
0x9f60d9574598a5af8de77cc86f249c62ff4d236d
0x2cac68d990ccdfbbcbe2e234bcb90c2150c5f1be
0x217fa6d15106ae33f8a75b9daf43595a515c234e
0x2b8b5a1d98252c68cce260b576cb84f9acd045aa
0x6260c1fc935599a677a5fbac62438de03278b05b
0xe0fea1f2210bd1980e7016f81d88b0464dd290bf
0xb327f7f16c42f02d94dc8385244503688c970d80
0x9f9475a257538748e5687ac5bab5577e373e1bd3
0x21b6ab1b8b328fff93050c844217a4773e294453
0xe3ef7ad6388dd64bb2e4bdb9e5022708ea89e374
0x25e6d7b6a6dbff4e9775f0988c4125ec1a65681d
0xf390b163c49c5fdf8558c8b3b73875b7f330534b
0xd663f2e1e3406de75955389828edf35d3fd60d78
0xe76c06d29ae2c8e79bc79a0c98ad790ed29f24d7
0x5360ad2429a9951d8f5300af9c55723d6a22d1d8
0x1dc4920df43267cd29e0d818974adb5a21229571
0x3b6108e62b8d5510113f351f169eb430e5ba55b3
0x752fa1ade9f79fab3ae88b10e88de3e5d3cac89b
0x5c149d9ee9b18a9e21e8e030d86c36d5c3e8eb9b
0x3036901bfc3ebef0c48a26bac89c2b5c599134f2
0xdef1af36de088efd74a81d37258f9ad91eed0e44
0x56d943fae1bf46eb0d805b98483a16cbebf9fdb5
0x97297f1515f246ccc0be01dc9d069b9f711a61cf
0x09ca229c1a374f91b7977923d9b61c25f3550af4
0x79d6ef2c52ef8a03f5644e811e47d7ad6b45daeb
0x98be3aef6e46951fcb1cf0b1f39b480053cfe90c
0xbdea2355a8c25b75e91911e57980c58aa4cfafe0
0x9ee799e77eb3d51671f6fbb942bcfe7d4225bc1b
0xc422ce9ddc00a6e6450419f15294886f74b6e623
0x3aeadc1cb286c9d876053a21fc3ea2efddd2085c
0x6e1860b986350b5f517c61b93aad0ccc05130e26
0xdd44f0945faf34b7bca10f3c3a799880f93eeb8d
0x2d1667ed37174f2552acd10e7deddc21ddbc7a8a
0xf2f5e1e935c83552c67cc7788cc58ac597c0dfe8
0x030ef5b6da73338d8562baa7b7c2768536662f04
0x2e140cec7bf6bc100a623bdb6c0cfb5ccb702879
0x9dbb29feaf43fdd27996dad525b9f23ca1119d6b
0xa23949a63e2ef3e99c3e855a981da5ed155ce00d
0x51dd886f05e7dd60472d5303663c5cdd971975df
0x78a856034f44b179ce6dcf77afbf65df9e21fc96
0x67301f46e13a1b5347e18005d80db551e026c217
0x252364d01045637d999a49578921cff17405a8ba
0xaf7b4019b96a1dd3f80c2b3e1725b291e75fe644
0x3191f765147f250a8022c0eaeb655128a00aeda2
0x6cd9fb23eb8c355e3150c830e908af3510a527bf
0x14c65434a74f42363f58b33f72487c8079e92b3e
0x898d35fcad782dbdb1e0bd99566a2eed1f1bc2e8
0x974d6f5b3939c2783cf61119b31e0db47cda3c51
0x7b817ddb14ef2d1cf8a0e4b4e470928518aaa920
0xcf97357500085e6cf8f8f37d5f47a05efecdaf79
0x7ccfb39cd2485d131645617a27c78745b38e1e11
0xc9f390a89b5ba7fc0d0a65c01e189147ace323dc
0x97af3cc72bf372bd39f1a1a5b642a4a3d129d3be
0xe5bd6d2f71e6aad61238cd1636b3a545ab61f6a1
0x32e651fb28164021dd47562d5ac69b5e97105376
```

<img width="526" alt="Capture d’écran 2024-05-16 à 11 27 24" src="https://github.com/ultratwo/sybilled20/assets/160050412/349f123d-7b83-48c3-960b-ed83954a93f9">




The addresses share the same on-chain activity. They execute the same transaction at the same time in order to farm airdrops accross +60 wallets.
 For example, they all provided the same amount of ETH (approx 300$) to Stargate on Linea the very same day.

<details>
<img width="639" alt="Capture d’écran 2024-05-16 à 11 09 39" src="https://github.com/ultratwo/sybilled20/assets/160050412/08b70a11-94e3-41c0-ae97-109e49fcddc7">
https://lineascan.build/tx/0xb4d8533a92f8d6f7f19f9cf807648cba04a8a65298b3ecb8f1e07dad8d517ecd

<img width="651" alt="Capture d’écran 2024-05-16 à 11 09 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/3241825f-2816-436e-b1c3-419f46498896">
https://lineascan.build/tx/0x3a4c32ddfee1d07262ebe2afb8e45730d9afe5c05d5ab91685992a04aaf2d19b


<img width="633" alt="Capture d’écran 2024-05-16 à 11 10 04" src="https://github.com/ultratwo/sybilled20/assets/160050412/dfb9e599-1e73-4799-9c2b-1a41739e2f20">
https://lineascan.build/tx/0x71d6ea40d910ec33e1b8769467f34308d728c8e1fc4ef753924191f08b421748

<img width="661" alt="Capture d’écran 2024-05-16 à 11 10 14" src="https://github.com/ultratwo/sybilled20/assets/160050412/1e397be0-2c15-47b5-8abe-f60a4a435630">
https://lineascan.build/tx/0xb14dacac5e59841d7c6e8c2b7678fce39f3709d4fe5943ebef1eac499e46cea1


 <img width="648" alt="Capture d’écran 2024-05-16 à 11 10 25" src="https://github.com/ultratwo/sybilled20/assets/160050412/5285bd68-2a97-4d10-88db-18dc9368b050">
https://lineascan.build/tx/0x130080966d279e94ea119d3e0c000e9c600c0ee298e195fc68947975597a8653


<img width="632" alt="Capture d’écran 2024-05-16 à 11 10 41" src="https://github.com/ultratwo/sybilled20/assets/160050412/a4f8ef84-19f2-4ac0-b324-dfb518bca7af">
https://lineascan.build/tx/0x28e055d74543c49ca39baf07ab254eaf51c619c3314e3f90f2c2798b4d41bacf


<img width="653" alt="Capture d’écran 2024-05-16 à 11 10 51" src="https://github.com/ultratwo/sybilled20/assets/160050412/110c0aa5-363e-46a5-9594-86ec3ea967b6">
https://lineascan.build/tx/0x77613eab34f3828fb87ccb0b1806c12b900575e8f817e1e7ab8644c5da55c970

<img width="636" alt="Capture d’écran 2024-05-16 à 11 11 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/6a5b3011-b561-4587-8ba3-cba3ddf7f682">
https://lineascan.build/tx/0xd879c999eb32a17aac2163a97b16a9418e721427784803d5de822762b27bc693


<img width="648" alt="Capture d’écran 2024-05-16 à 11 11 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/5778a31f-57a6-498d-856a-3dbcdfbd5ff2">
https://lineascan.build/tx/0xd923e1b8b0824e9603c298194c88c6b606626381272a1e66a4094c4ee52b745f



<img width="653" alt="Capture d’écran 2024-05-16 à 11 11 27" src="https://github.com/ultratwo/sybilled20/assets/160050412/4b1ca065-49a5-463a-a578-54e01fde6b63">
https://lineascan.build/tx/0x373861ba707ab06a5c6b8fa0488f4182c0de609ca536b5d5b03020e9d9a12c5f

<img width="615" alt="Capture d’écran 2024-05-16 à 11 11 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/26411fd0-762a-4327-9d9f-d11bfdb9300a">
https://lineascan.build/tx/0x6c3b3be5af94c5932a4e72b2d776967cd52d398b7975a96d15d179636029ae08

<img width="648" alt="Capture d’écran 2024-05-16 à 11 11 57" src="https://github.com/ultratwo/sybilled20/assets/160050412/9c05d99c-e730-4a31-a561-648687b5b2c4">
https://lineascan.build/tx/0x700b2091901d9c9750c4519e46cafed8e1e019ac84c05c448039b37d87dac6a8


etc...

</details>

This goes on and on, for example they all used OpenName 4 months ago on ZkSync (L0 interaction). Another example is they all used Stargate from BSC the same day in Feb (it's their last L0 interaction before the #1 Snapshot).

<details>


<img width="645" alt="Capture d’écran 2024-05-16 à 11 16 04" src="https://github.com/ultratwo/sybilled20/assets/160050412/4779da75-7535-4411-be66-cbd006c56c64">
https://bscscan.com/tx/0xc5f0afa0f37e9a89e5273d729dd96426566d800c0a64404bf01a165ca89ad1d6


<img width="655" alt="Capture d’écran 2024-05-16 à 11 16 14" src="https://github.com/ultratwo/sybilled20/assets/160050412/74c5dac9-3287-4cec-b47e-fa8e0c8cdda2">
https://bscscan.com/tx/0x88deb203f3b37b6d9b86941135e1634865a54eaa646b456da80fc42d0d2301f7


<img width="621" alt="Capture d’écran 2024-05-16 à 11 16 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/20bfc18d-c1d5-4120-87f2-0fe33a70ec8c">
https://bscscan.com/tx/0x2db1eb85e3e96db976f0921a9ee3e162c2d99a70d8b64d4c443235db26d6b8c7

<img width="668" alt="Capture d’écran 2024-05-16 à 11 16 34" src="https://github.com/ultratwo/sybilled20/assets/160050412/c9a96483-9c96-4087-95a7-b396db18307a">
https://bscscan.com/tx/0x293e6cd7a2ecf6928471e9eb6060e871f5b5980db486b5924561c6e783e4fc2f


<img width="671" alt="Capture d’écran 2024-05-16 à 11 16 45" src="https://github.com/ultratwo/sybilled20/assets/160050412/1ac8ba8c-bf81-4881-a0ca-dfbe61f98bad">
https://bscscan.com/tx/0xbe07daeeac495e1d1f90543106205bd3e35dbedd0c821eb8725fe2a7012775bb

<img width="636" alt="Capture d’écran 2024-05-16 à 11 17 25" src="https://github.com/ultratwo/sybilled20/assets/160050412/9834a74b-196a-4616-8594-fbebf80f9de8">
https://bscscan.com/tx/0xe54e55c9582e9dc0b95c22cb5c0d2218f8d5242ecf4a17b485ad24c4cbe50f10


<img width="643" alt="Capture d’écran 2024-05-16 à 11 17 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/0d0a0751-886f-4a44-a88e-df091e0d07f7">
https://bscscan.com/tx/0xb657cb6539987a488faa8826d37abf34c33e8cadc41e81e865a7a04ad87f00e2


<img width="631" alt="Capture d’écran 2024-05-16 à 11 17 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/c902a619-69a1-49c8-bbcc-4db123b79ec3">
https://bscscan.com/tx/0xb42e89c2e84215c9578f58ceb6fef9c651d85b5bd453a5e3520561f3f255bad1


<img width="656" alt="Capture d’écran 2024-05-16 à 11 17 57" src="https://github.com/ultratwo/sybilled20/assets/160050412/c47aa234-4e35-4925-9895-7bcf0314e176">
https://bscscan.com/tx/0xaa7d86baf9ec6e3cdb8a08723dffb3eeaddaf55a9af20483693e7f5aca34897d

<img width="677" alt="Capture d’écran 2024-05-16 à 11 18 10" src="https://github.com/ultratwo/sybilled20/assets/160050412/bb6fa19b-d75e-4869-9c06-09763d170a5b">
https://bscscan.com/tx/0x051ce96f5a9cd7fa92488ed143f37b45ae2eabe4ba9e5314c8a7a64135ad123a


<img width="642" alt="Capture d’écran 2024-05-16 à 11 18 32" src="https://github.com/ultratwo/sybilled20/assets/160050412/9c48c335-9e66-437e-91b3-7c1af399c89f">

https://bscscan.com/tx/0xea0fe5d853d29a88076a850d31bb6df319cde90c086aa41be86b97ab8e395cff

<img width="651" alt="Capture d’écran 2024-05-16 à 11 18 41" src="https://github.com/ultratwo/sybilled20/assets/160050412/564167fb-c576-42d8-9dd1-318ca1ddb075">

  https://bscscan.com/tx/0x6570785e3c7b901ada6e4007d4f4bb0d3a8205975a84ddc88fd18707e4dcaed2


  
</details>

Cluster + same CEX deposit address + same on-chain activity at the same time, this is without a doubt a sybil operation.






## CLUSTER 3

The first 9 addresses of the cluster share the same OKX deposit address 0x0d5eA059602029Dda50c3DD96609d086307e2E3A. The rest are linked to numerous addresses of the cluster, multiple times.

```
0x4b5697d5b87a0c2d8410f1adc4124684c4e3c5b0
0xad0c8a1502c5e227fb37eb95624fbd4116c2ff02
0x3678638b035b7e9d55bdb8db25063c716b1d111a
0xcfb4fc3f5f7e27131f4b0304ba48a9f5942c8f62
0xe27802c0dd343876147b6b388878d90e4e7f3143
0xb31bf9e27e426b2686cd084ba95c2f9d40ba2b64
0x8f85d6fa16fa2b8d585c952d6c67e7b6bb85ab13
0xb775756abd562c488d12d308ff42e466f8a64cf6
0xdfc5e25a3d22eefedf8e8ad15cd45c0a262a7f2b
0xc8502840918a2dbc6554678a27dee96261acd090
0x6cd2aea05f8457723e22faa95d298079e895d504
0xeb741ffb2691c867a77be5fe4d7a31f69a453a1b
0x0b13cc3dd683d022aa90bbcefa6c101032f759ec
0x27f0f8f3827645613b56e63ea20b0139cdba5efe
0xdae404b52c5c3b9af2a4029937554f656eb128f9
0xb40909cf519adce0da10bcbfbfc6e29e626aab37
0x200210d9ee8356055e887e7ee96d4333d8f2ed38
0x57e428c3e44a5e9639758d580130a48a96977286
0xb85038ff4676671c21726072d9530863eeb537e0
0x62f555234acc289bab410a37a83c705cfb00d7b6
0x7cb326cc75cd1933be37583004ca28797b10ffbc
```







<img width="614" alt="Capture d’écran 2024-05-16 à 01 11 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/ee57cdc3-ac44-4e7c-8def-69ed799aaed4">


The addresses have the same L0 age (date of first L0 interaction), 197 days ago, aswell as similar amount bridge, contract count, number of unique days/weeks/months etc...

<img width="1103" alt="Capture d’écran 2024-05-16 à 01 12 48" src="https://github.com/ultratwo/sybilled20/assets/160050412/d518305b-6371-45bd-8497-d1073fda4a63">


The addresses have the same on-chain activity. Their L0 interaction are the exact same, the same DAPPS in the same order in the same timespan. For example, their latest L0 interaction all are the same, and follow the exact same pattern : Aptos Bridge, BTC.b, Merkly, Aptos Bridge, Merkly at the same moments. This is the result of a script.


<details>
<img width="900" alt="Capture d’écran 2024-05-16 à 01 08 13" src="https://github.com/ultratwo/sybilled20/assets/160050412/5b7852ef-216a-49ca-b48e-e7afeac9317e">

<img width="890" alt="Capture d’écran 2024-05-16 à 01 08 20" src="https://github.com/ultratwo/sybilled20/assets/160050412/e013ab25-0eab-44cb-8c25-17c59c9f704f">
<img width="887" alt="Capture d’écran 2024-05-16 à 01 09 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/88c7fa97-95d2-42c7-b516-769b03e0a92c">
<img width="911" alt="Capture d’écran 2024-05-16 à 01 09 28" src="https://github.com/ultratwo/sybilled20/assets/160050412/c8cf7dbe-f90d-4559-aab4-05bdcbca7648">


<img width="905" alt="Capture d’écran 2024-05-16 à 01 08 26" src="https://github.com/ultratwo/sybilled20/assets/160050412/f83664b7-5f04-49ce-a1ef-23788b2e563d">

<img width="908" alt="Capture d’écran 2024-05-16 à 01 09 00" src="https://github.com/ultratwo/sybilled20/assets/160050412/2a230fda-b81e-42d6-aee6-847d6874c224">

<img width="913" alt="Capture d’écran 2024-05-16 à 01 08 33" src="https://github.com/ultratwo/sybilled20/assets/160050412/b8a4be0c-d100-46a5-a7a4-41fb0f872c34">

<img width="908" alt="Capture d’écran 2024-05-16 à 01 08 39" src="https://github.com/ultratwo/sybilled20/assets/160050412/f84cadb4-7982-4fb4-8194-17d4ea5ddb2b">

<img width="883" alt="Capture d’écran 2024-05-16 à 01 09 17" src="https://github.com/ultratwo/sybilled20/assets/160050412/1560ae0f-80c4-4140-832e-51bd5ba6b6bb">
<img width="903" alt="Capture d’écran 2024-05-16 à 01 09 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/00c191c0-b7ee-4964-a572-4c05eea7b0ad">


<img width="910" alt="Capture d’écran 2024-05-16 à 01 08 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/37aa86ca-25e4-47f0-aac7-21901bb432c6">

<img width="895" alt="Capture d’écran 2024-05-16 à 01 08 54" src="https://github.com/ultratwo/sybilled20/assets/160050412/53526caf-d3fb-40d3-b674-8f46597415c9">

etc... 

</details>


Same CEX deposit address, cluster, and exact same pattern of interaction with L0 to farm the airdrop. This is a clear sybil cluster.





## CLUSTER 4

The first 9 addresses of the cluster share the same Binance deposit address 0x890B073a3aF6278aEf6eA14A0D99256Fb4C358C4. The rest are linked to numerous addresses of the cluster, multiple times.



```
0x9e69f8b30edec58cbf3b6f43bc737ad524690a33
0xcc2e4839f2972055474bacbcfceeee77af52bc84
0x05f4bb916a16758ed1f8b4a8abbb786a28a6bfa7
0xf05e9e8daa2c8844c67e7532f055e17614ec90da
0x226d4e9559b91a58f5763d11722178a983e8efd6
0xcfdad50192904eef83ba0a1140d439bdef641a9d
0xd7141879a66eec05b47298da947ee1eb3faf0906
0xc116b2a3025c23f0a208352a84421ff379aab790
0x7dfea24e27488ff1ac7ddc6985997699cee9f26b
0x499029530f09d7585f01ac18ec6a68b6c0fda059
0x1960d4ef14c3b576d821d3bd475ed6034a2e6c0a
0xa71b0c2d4bc5e92b06688d70147d184c6ddc8c5d
0x342d694377f431da175bc1317046ab424a612cd8
0x03cb82fc93b3e79774570fa7661fa34b63b0b805
0xd4bde8529173d64fe5c16bedd34475caebe8c57f
0xa66aa01250328d68c1c37bfe83bb211b9c1b71b5
0x21aaf5677556addf1e6cb6cc38ebdc131c47d5a0
0x43759f32b7da8acd09345a6ae8e30d7b81181160
0xa4b3b9b79147995d0b868fb121cf4c26a387416c
0x1d9186201b353275edc4a5d57841fdce8b70b263
0x396ab568329d36346f1d9a62df6212ad31316682
```


<img width="585" alt="Capture d’écran 2024-05-16 à 13 52 10" src="https://github.com/ultratwo/sybilled20/assets/160050412/353296b8-9891-42c2-8aee-64bc8c15bb83">


The addresses have the same on-chain activity. For example, their L0 interaction follow the same pattern. They interact with the same dapps in the same order in the same timespans.


<details>
<img width="908" alt="Capture d’écran 2024-05-16 à 13 54 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/488e8bf2-6a84-45ec-a0c6-446dce8e6cc7">


<img width="906" alt="Capture d’écran 2024-05-16 à 13 53 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/367fc352-999f-489b-a657-660dac2a3815">

<img width="899" alt="Capture d’écran 2024-05-16 à 13 54 20" src="https://github.com/ultratwo/sybilled20/assets/160050412/55591296-2bf7-4e2e-b6c6-cf6f4afa7451">

<img width="894" alt="Capture d’écran 2024-05-16 à 13 54 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/5276df8c-fd4d-4aad-9cff-392266b999bb">

<img width="880" alt="Capture d’écran 2024-05-16 à 13 54 14" src="https://github.com/ultratwo/sybilled20/assets/160050412/a1106cec-480f-493c-8f80-b1611f9f4d0c">
etc...

</details>


Another example, all the addresses of the cluster locked similar amount of STG (<5$ worth) in November 2022 on Stargate Arbitrum, and used Stargate on Arbitrum to bridge the same amount of STG the same day in November 2023.

<details>

<img width="647" alt="Capture d’écran 2024-05-16 à 14 00 39" src="https://github.com/ultratwo/sybilled20/assets/160050412/68228d31-f155-4d19-bece-1738c90cd1f1">

<img width="639" alt="Capture d’écran 2024-05-16 à 14 00 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/d8f3c58b-ddbd-4a58-95b4-2dc38a7f838b">


<img width="655" alt="Capture d’écran 2024-05-16 à 14 00 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/2fc00e3c-64a4-4941-bfde-8b9814a2bad3">


<img width="631" alt="Capture d’écran 2024-05-16 à 14 00 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/97bfd36b-05e9-4341-8733-dff5c0dc5c52">

<img width="653" alt="Capture d’écran 2024-05-16 à 14 01 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/2cb44271-93ba-4f6a-bc68-33717716c154">

<img width="635" alt="Capture d’écran 2024-05-16 à 14 01 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/debcdb0c-5411-4da4-bafb-460422a6f302">

<img width="640" alt="Capture d’écran 2024-05-16 à 14 01 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/b302a84b-9cab-431f-848e-12f918c76c16">

<img width="642" alt="Capture d’écran 2024-05-16 à 14 01 22" src="https://github.com/ultratwo/sybilled20/assets/160050412/8737b394-aec6-49f5-b3f2-89ca5488d457">

<img width="635" alt="Capture d’écran 2024-05-16 à 14 01 42" src="https://github.com/ultratwo/sybilled20/assets/160050412/81436860-2081-4a0c-b844-36eeb50ecf47">



<img width="642" alt="Capture d’écran 2024-05-16 à 14 01 31" src="https://github.com/ultratwo/sybilled20/assets/160050412/f398b05d-284f-468b-b594-fa5b6417fbcb">


<img width="669" alt="Capture d’écran 2024-05-16 à 14 01 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/0eb994fd-f85a-4f3d-9071-a3051b518986">








  
</details>





Cluster + same CEX deposit address + same on-chain activity. Without a doubt a sybil cluster.








## CLUSTER 5


The first 14 addresses of the cluster share the same OKX deposit address 0x5510E75E1453735A42c406d8e576325975387821. The rest are linked to numerous addresses of the cluster, multiple times.






```
0x772c1b29e66d6d6dca8fd3e8de3c3a6a38367253
0xa61ed32bbebefd59f7247707aa37d4155157f877
0x6ff9818b712c7d7cc857cdc0577c75075ad2ccb0
0xe1f43c9e7636ed8180c599286c050b3fc8c11df9
0xdda6d8569730d2a502845d98fe1f037da16bd5d0
0x3c5062e7b9980139db30c642981cd2f6c0c2a4fc
0xb35d9c51703ec1c55ae6a46f84cd730c9b1bf675
0x4838ee9017eef2ab92ae0abb236874a1264a6ae5
0x3dc3edfde4fa8f5e766f706d8f7c686c66dda02b
0x365aac4a0b7f85286c7f1f803509017ac8a8d71e
0x65d79080c25c7640c7279706ff0a81dca7c21ea7
0xcb5e405b9662e91d100388fc73eeb139c3171968
0x42108c3bc2b0021857847a3948f80772fc7d8e0e
0xa1b29f7749abff66cdae533d20608c3b77e8bab6
0x2a76d4c7cfed6021b544b3ffb7d320a0ac7ca365
0xc81b9cb36dfd30676f06eb9af21f71c2a0738e8a
0x1f63e5f7a689db1f8060b6b280ac84ab852e95a2
0x400c158c656818ccbd194e013edcc0fd3e7e839f
0x1cc34af24c9ac2fce2f3a29b01cd6d0b9eab6d15
0xe5ec946d8c7758115f79a74653529a9ca4aca6ca
0x17e87f44fe6d9231af6e537c8a6b61ec4398794b
```

<img width="563" alt="Capture d’écran 2024-05-17 à 16 30 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/f86f525e-fc57-4523-af22-9e5feff0a9e5">



The addresses have the same on-chain activity. Their L0 activity follow the same pattern, probably the result of a script. For example, their latest L0 interactions all follow the same pattern, starting by most recent: an Aptos Bridge transaction from Arbitrum, one/two BTC.b transaction from Avalanche or BSC, another Aptos Bridge transaction from BSC, and Merkly transaction spam from Polygon. The date of the transaction also are similar.




<details>


<img width="893" alt="Capture d’écran 2024-05-17 à 16 32 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/8f902dd8-1d6c-432c-9abe-3f1b0aca0fe4">
<img width="898" alt="Capture d’écran 2024-05-17 à 16 33 13" src="https://github.com/ultratwo/sybilled20/assets/160050412/470c9f3f-04c3-4e67-bce7-3c2e8e911ce8">


<img width="902" alt="Capture d’écran 2024-05-17 à 16 32 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/0fc9a695-cb4e-46fb-9c72-e3ee42425912">

<img width="899" alt="Capture d’écran 2024-05-17 à 16 32 28" src="https://github.com/ultratwo/sybilled20/assets/160050412/486d9a83-711d-4c8e-b19a-0cfd88c9445e">
<img width="895" alt="Capture d’écran 2024-05-17 à 16 32 40" src="https://github.com/ultratwo/sybilled20/assets/160050412/2b3d85e7-0413-4136-8f85-fe8c8c6df806">

<img width="879" alt="Capture d’écran 2024-05-17 à 16 33 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/29717e8a-2e23-41c9-bff8-e4171f6216b2">

<img width="908" alt="Capture d’écran 2024-05-17 à 16 32 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/ecbc2503-43bc-4a2d-a349-dcf8a3ebddfa">

<img width="908" alt="Capture d’écran 2024-05-17 à 16 33 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/61a5c800-6cec-47f8-9898-ba8169b4ef06">

<img width="906" alt="Capture d’écran 2024-05-17 à 16 32 34" src="https://github.com/ultratwo/sybilled20/assets/160050412/f898f3c7-ce35-445e-99b3-fe989237094e">

<img width="889" alt="Capture d’écran 2024-05-17 à 16 33 19" src="https://github.com/ultratwo/sybilled20/assets/160050412/e99c2781-6668-415a-82e5-7e4fceaeb279">


<img width="882" alt="Capture d’écran 2024-05-17 à 16 33 34" src="https://github.com/ultratwo/sybilled20/assets/160050412/54a7b565-e7d4-40b3-a458-e3435922f726">

<img width="890" alt="Capture d’écran 2024-05-17 à 16 33 40" src="https://github.com/ultratwo/sybilled20/assets/160050412/bff43b20-61c3-4f9a-8b98-918b462dd28e">

<img width="905" alt="Capture d’écran 2024-05-17 à 16 33 45" src="https://github.com/ultratwo/sybilled20/assets/160050412/d3b3c770-7029-41b5-83b5-20aaee0be504">


<img width="897" alt="Capture d’écran 2024-05-17 à 16 33 50" src="https://github.com/ultratwo/sybilled20/assets/160050412/e6c3c67a-d222-4f08-8712-6d28fc18a928">

etc...



  
</details>

Cluster + same CEX deposit address + same pattern for the addresses of the cluster (result of a probable script). This is without a doubt a sybil cluster.









## CLUSTER 6

The first 25 addresses of the cluster share the same Binance deposit address 0x33F820BF7eFd42A6E38f9f79E03b61713A70EbcE. The rest are linked to numerous addresses of the cluster, multiple times.


```
0x03C12E6683bc893464E23364998207B6F12ffbE2
0x850b87d03a705cfcbd46b1be9a540ac4f553a032
0xf25dd21EC783Ca3f0E426b008587821848804d25
0xa5442684505b8eae70D76b5F3E907856718747Ef
0xACA0FAaE2E4f1bE30B68a1A5c9b1D00be5530a5E
0x778614602f591b1458ae916b9cf5bfe9d504dbaa
0xaffbdb5e2fa03ab8a28fa39ebd6bfe94386137ce
0x6cee3A2E8E2d95B3fdf2FC6974E05c6f7e8301B4
0x1b85c8f66A84A48e7db60Cb915701dD768E6EBF5
0xC83A61d44474e929aF19B7d2102d3BfF6f1B4B2c
0x1E3C4fB112a999a0625bD31aEE063DC61a0dB3f4
0xc092C150466fDC64516DF925f12Ff699dD82a35D
0x0291844A8Fa14be573f03C49FEe394Dd21059146
0x29Ab68f27936F5C45Da7c1DEdcD2598aE13b64D6
0x7BeFD9252fB9CD99d3D9C1A33a01bc9F36E9283C
0xB5ED77029151C44Fa5D9BBE83647fdF7E989Dcc4
0xec613ab9a2df9ca12ae0d690e95efcb075505ff9
0xbe672f5e21cdc8a0849212b1ed54d8145a52fcd4
0x1d981567d01645697d28d0c1c6eb7e06ed4a2e39
0x6b7ecadd2b458f2b77a50557fe231ad20a7c9846
0xa557f04397227948db25a3a81ece5285ec538f0e
0xda1259aa131dfe437d50072d929f925d1f2e6e89
0x719e17d2dc72f048c258f48331ffdc284f29c667
0xdb8eb81293ae6c6d8ff8fe3de740f38b462fb9e2
0x9bd226eff925470f5671181daf17fd4661580805 
0xf8505850b5de03a79e17844f6396d2985b1ee8ff
0x40bf75304596ca5ce424f6cc70cef7cae5ad8af2
0xaf36e4f1faf80c2426be4566bd4adb753848b0a5
0xe0dd2b8196aa0b67a831ef7712b475e4e23ed3cb
0x7910e22bc044041efc81ca5522a36507e307ac67
0x7c87886de6bd71e88427d2f64aaaadf8887fd1e6
0x6084433b07d4466541af1cb5c3dfd7a50fdbb57b
```

<img width="474" alt="Capture d’écran 2024-05-16 à 00 33 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/2b251f1d-2cb1-454e-9ada-16fa2e263a35">



The addresses have similar on-chain activity. For example, they all withdraw similar amount of ETH from OKX in the same timespan (7 days) before using the Scroll native bridge in order to farm the Airdrop accross +20 wallets.


<details>


<img width="655" alt="Capture d’écran 2024-05-16 à 00 34 55" src="https://github.com/ultratwo/sybilled20/assets/160050412/a5b55fbd-2498-4164-b383-75c4c9419401">

<img width="662" alt="Capture d’écran 2024-05-16 à 00 35 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/85f576f9-3120-41f4-94ae-358439239449">


<img width="656" alt="Capture d’écran 2024-05-16 à 00 35 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/754588ab-4502-4249-8123-94f3fb04ca90">


<img width="652" alt="Capture d’écran 2024-05-16 à 00 35 21" src="https://github.com/ultratwo/sybilled20/assets/160050412/f79a5080-3862-49cd-9bf4-0a720bf4ebdd">


<img width="622" alt="Capture d’écran 2024-05-16 à 00 35 29" src="https://github.com/ultratwo/sybilled20/assets/160050412/5f64e223-928d-4b02-aaaa-1cb410b47ac2">



<img width="624" alt="Capture d’écran 2024-05-16 à 00 35 38" src="https://github.com/ultratwo/sybilled20/assets/160050412/5711c448-e6a9-4c25-b1f8-34af37f41759">

<img width="633" alt="Capture d’écran 2024-05-16 à 00 35 44" src="https://github.com/ultratwo/sybilled20/assets/160050412/21cf2615-a72a-44cc-8571-a1ecfde6140c">


<img width="631" alt="Capture d’écran 2024-05-16 à 00 35 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/b636c06b-d9f5-4c82-a5e5-e1f12754a043">


<img width="628" alt="Capture d’écran 2024-05-16 à 00 36 00" src="https://github.com/ultratwo/sybilled20/assets/160050412/65ad62ee-5a14-41d7-8dac-00eadb4a9e47">


<img width="676" alt="Capture d’écran 2024-05-16 à 00 36 05" src="https://github.com/ultratwo/sybilled20/assets/160050412/f8739daf-a4b0-44aa-8e39-a65cd72a7e2f">


  
</details>


Another example, they all locked the same amount of STG on the BSC on the same day in order to farm the L0 airdrop.


<details>


<img width="719" alt="Capture d’écran 2024-05-16 à 00 38 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/5ed36d57-da66-4a6b-84b0-bae0a3d7b3a4">
[
](https://bscscan.com/tx/0x4718650bc5cebb02502fc0f9f9d027ecc10f6c4d0e0413a16a830588e721d4bd)
<img width="644" alt="Capture d’écran 2024-05-16 à 00 38 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/8cfa2d35-711a-4365-ae89-09034667b7b9">

https://bscscan.com/tx/0x7b4a34dc19e85fbfd31e15ca753501d3f1c96a1aa626f3cc865a0bcf4f8af764

<img width="635" alt="Capture d’écran 2024-05-16 à 00 38 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/cd224e06-4765-4cfa-8181-725482e9397e">
https://bscscan.com/tx/0x7e9945d3099a216289a1bd5113ee5722288d438b27e30494fe532fd22df4efe3

<img width="650" alt="Capture d’écran 2024-05-16 à 00 38 53" src="https://github.com/ultratwo/sybilled20/assets/160050412/96514e0a-5954-41d1-af2b-32eb28a4442e">
https://bscscan.com/tx/0x270d577c431d13596e90bb4fe223e4a8b59ae38713bddfbcda7accf6c4422372

<img width="662" alt="Capture d’écran 2024-05-16 à 00 39 03" src="https://github.com/ultratwo/sybilled20/assets/160050412/badef2a9-f386-49f1-b93a-d0b1001f26bb">
https://bscscan.com/tx/0x3b93e7c06ff1b371b99dbf934a45b871f5cce799cfdfed6ef19376bc569291d7


<img width="646" alt="Capture d’écran 2024-05-16 à 00 39 10" src="https://github.com/ultratwo/sybilled20/assets/160050412/e275f9ad-6b4b-4385-b1cd-22eda7cd1253">
https://bscscan.com/tx/0x185e65df81790298324da94f49d72a17fa81166df813f98bd761a1a4de1de0c9

<img width="667" alt="Capture d’écran 2024-05-16 à 00 39 17" src="https://github.com/ultratwo/sybilled20/assets/160050412/7439dd2b-f08d-4275-b323-c5f5d83eff3e">
https://bscscan.com/tx/0xc7a895a2e491fe6409134408eed97ea5775999a037b186f56110ce3bcc4107ab
<img width="629" alt="Capture d’écran 2024-05-16 à 00 39 24" src="https://github.com/ultratwo/sybilled20/assets/160050412/b5fa98b0-7e6b-421f-88c6-4525238473f6">
https://bscscan.com/tx/0x7491cfee3b2a98016c6f8d91d33fed600203331f6175492c1e0d5c2debf01fd8
<img width="655" alt="Capture d’écran 2024-05-16 à 00 39 30" src="https://github.com/ultratwo/sybilled20/assets/160050412/2dec955c-3bd9-4e47-a61d-c2cd35d697de">
https://bscscan.com/tx/0x65869d9066f52b545549c81da91bd5f4cb2230daeb740fe4347ac541c0af566e
<img width="669" alt="Capture d’écran 2024-05-16 à 00 39 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/9ba259f9-b91d-4be4-a6fa-6b8ee175e490">
https://bscscan.com/tx/0x62675a3e8a3dab8830506d6620f2196e0b2fe811417231f5482ab72f77682614

  
</details>

Same CEX deposit address, cluster and same on-chain activity. This is a sybil cluster farming multiple airdrop accross +20 wallets.



## CLUSTER 7


The first 13 addresses of the cluster share the same Binance deposit address 0x524F9395C3fDa99324EC365e42Bbca4C2233905D. The rest are linked to numerous addresses of the cluster, multiple times.

```
0xfa4dcd9854bcf0ecd6ee277a3811e667aaf9a31d
0x6b8dd1d1efe8c44c9849a945a228799be488db65
0x9bc975d6f11d24615e01e34de027b2dcd7bc32bee
0xa09b1f358ac758f0f350244a98ce1548ad820674
0xd10722306e7558fc1aa45cf5a32e694405fe67f5
0x7432cedbbf8349dbf7063685ddb86fbd28750639
0x74eaf9a43f66463ee297877bd8177dca0a991733
0xb4281c847d4e934a61b4b76fbba20a905ea1ec0d
0x7b40814d92dd3166ded02495d8e34916fea22538
0x9e36d77c030e38cf5dba9d392a6df8c441444027
0x8e6cee522a0356700021981fafe0a46a10e702fe
0xeacb1223184267df749afa9bbca4d7606ba57306
0xc4ad86a5f369d3fe935af8453b78ea8f07685b98
0x4e0803877f75984f52c0a7321ed89cc517dc82a5
0xef7a2237ad19b8e12a1ca233ccc2d0ee4bbe050a
0x0dc4b06314bad7afcfd7bed18e086d8b98c75f8c
0x840ed7151250bf16bcdd185f8d15e72760f966cc
0x22224ff41ab18a841b629afcdb95559f7ba07458
0x3118835f40fcd9f0e0ccf9a043918a8dad6368ca
0x090ceb8557454ef92a926e5c0852ad5599c0ece3
```

<img width="512" alt="Capture d’écran 2024-05-15 à 16 39 53" src="https://github.com/ultratwo/sybilled20/assets/160050412/98372e1c-a603-46f4-9439-fdf55fc7b594">

The addresses of the cluster share the same on-chain activity. For example, they all used the Angle Protocol bridge multiple times in a 4 day timespan to bridge EURA from the Gnosis Chain.

<details>
<img width="770" alt="Capture d’écran 2024-05-15 à 16 35 38" src="https://github.com/ultratwo/sybilled20/assets/160050412/6eda9bc3-82d7-46e1-9768-3ebdc0bc361b">

<img width="770" alt="Capture d’écran 2024-05-15 à 16 35 53" src="https://github.com/ultratwo/sybilled20/assets/160050412/dda37e3c-c3b3-40ec-af8c-9fe459d4227c">



<img width="801" alt="Capture d’écran 2024-05-15 à 16 36 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/f7886da2-419c-4ef8-b981-a42cccd690f1">


<img width="782" alt="Capture d’écran 2024-05-15 à 16 36 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/f82aab94-fbe0-42be-8192-3f00baa2cf73">


<img width="779" alt="Capture d’écran 2024-05-15 à 16 36 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/39c9a286-6a81-49ac-b415-d09c39c50b16">


<img width="783" alt="Capture d’écran 2024-05-15 à 16 36 17" src="https://github.com/ultratwo/sybilled20/assets/160050412/848149a0-a95a-4f6c-8213-b0350b634aa3">


<img width="767" alt="Capture d’écran 2024-05-15 à 16 36 55" src="https://github.com/ultratwo/sybilled20/assets/160050412/73da383e-d669-4ec0-b87c-a27dc3c3d8a3">

<img width="782" alt="Capture d’écran 2024-05-15 à 16 37 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/1064c14a-c32d-4370-b554-281107cbac69">

<img width="772" alt="Capture d’écran 2024-05-15 à 16 37 06" src="https://github.com/ultratwo/sybilled20/assets/160050412/256a137d-8ffd-429c-bc44-2c9569c37998">

</details>

This can go on and on with other blockchains and protocols.

Same CEX deposit address, cluster and same on-chain activity.



## CLUSTER 8

The first 7 addresses of the cluster share the same Binance deposit address 0x80d4780F924D3888a88825142A3785503B185F29. The rest are linked to numerous addresses of the cluster, multiple times.


```
0xf9fe62e107d8afa27b11c1f337ad2cca6004a0f5
0x42f19bce273dcf24697b347cfbd7e935c7042e58
0x8cca361f084cf1391b3a22d20e3a1ec7a80424e7
0x2b767ab20b28d2e63b677c50a9ceb36d178e33f7
0x5818f3d225024483c54722c3190c87a3a44aaf05
0xf1cc050147fcb394452c2f3cbb5743ea6a989297
0xd6029cc67a10219c6f799720925ca3f3fe8eb5e2
0xf34bb4b391ccdae754378014e19c5439d4f58661
0x016c53e77fc0bfeaf207b96f065974f91c4a80e0
0xc131af35470300f5538ec58fb3293b7642cb5426
0xeb33eab93cb6891f4684a01bf0d8547efc1fccfe
0xba7b63a9b32b03847d51de7e30fe30bc8910f76b
0x19aedcdd30289d10f8a23f1cf2e39a00320cc975
0x15e9fbea79121c90d8d7ffd8641e5bcf75935c29
0x876612ca89ba2047775c7892750d9b22012ab4af
0xfcacc4850862b6a5309a09a772756903e1f3c0b2
0x6d939d65d214dddbcbe1dd5884a7c9177d2b21ff
0x0511c0175cfc5819c84e586861aae90be1db3ee9
0x27ecf7524bae60c1d15b6b476132db93463ca809
0x1170599e563e4fbc6dc0e01e321a9f6256be7437
0xb84afad15c7615d13d811fae371d1ddb5dbf9212
0x4e6fbd80dae3e279de272ab8cb722ffab6748615
0xb2dbf47ad46c9df52964bacdaa7796b7cd82a0ad
0x0524a0b9b45bab07d62b637619356f83429e3511
0xee24d738d320c34d15b05d2548fb1a7e92ca959f
0x67ad2fe8d1b21323f58d0100ab8f702452b49d09
0x5f32b2580de517bf5b3292ab2c349020917b8396
0xa75e2f2a97c6dd26789b56db5d28a7e587ba6d9a
0x2698f1dfcec4db1738d8f6959b12174ce1a6ecab
0x76b7c6f584edd88656d3dc775003a44cd65afb42
0x558889102a60af6d0f46f45bcf19b0c196f1ef15
0x6c7526f129e79965a915a2463cc57cb08e828ba2
0x8e5c52ccfb7ee7fc00b5cca7e32a2ec457668f1e
0x02dd43f1affc63902ffa5772769414f2b774defe
0x050597ba475113931fce989b45a8b8a19a73b646
0x52d58545007b99d9c42a2a4907624f7d91cca749
0x9b850b96fb66a13361b4a4e2c7d8c20a9d802c8a
0xe65bcbae6aaf9ea55463157b05f83915834aeb61
0xb8a4c19512c088bcc2f71a6d785ee64de3570ed6
0xfc21d3a2465a220c5a5a35e99e423c612f76ae83
0xbdb52c7f622c44195c55c6f96a41f7a5facecaa5
0xa81036d740109d7f5720aaa4e93a5dc86ee94ecf
```


<img width="515" alt="Capture d’écran 2024-05-15 à 17 03 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/7ee28556-c6fe-43db-b078-0093648c91e6">

The addresses have the same on-chain activity. For example, they all locked 2 STG on Stargate on the BSC. Another example, they all used the Aptos Bridge from Optimism to bridge dust of ETH (<1$ worth) in April 2024.


<details>
<img width="764" alt="Capture d’écran 2024-05-15 à 17 04 39" src="https://github.com/ultratwo/sybilled20/assets/160050412/b9fabd94-e2dc-40cf-a28f-860e6ee1e24c">


<img width="764" alt="Capture d’écran 2024-05-15 à 17 04 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/36508ee9-943c-439e-be15-c68cef010832">

<img width="772" alt="Capture d’écran 2024-05-15 à 17 05 04" src="https://github.com/ultratwo/sybilled20/assets/160050412/29581ce1-9d08-4bed-89a5-9d3daf5a5d76">

<img width="765" alt="Capture d’écran 2024-05-15 à 17 05 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/0d5ed1d3-1668-45b9-b4d0-129691e64e55">
<img width="768" alt="Capture d’écran 2024-05-15 à 17 05 20" src="https://github.com/ultratwo/sybilled20/assets/160050412/10a95340-36dc-4838-87b1-1eaae4020018">

<img width="767" alt="Capture d’écran 2024-05-15 à 17 05 28" src="https://github.com/ultratwo/sybilled20/assets/160050412/0142de05-091b-431b-b745-cc03cf818e69">

<img width="758" alt="Capture d’écran 2024-05-15 à 17 05 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/08c352e5-c72b-479d-8e90-9be1d0619512">


<img width="760" alt="Capture d’écran 2024-05-15 à 17 05 43" src="https://github.com/ultratwo/sybilled20/assets/160050412/314300ea-42b0-46ab-8550-f365d01fea71">

<img width="771" alt="Capture d’écran 2024-05-15 à 17 05 50" src="https://github.com/ultratwo/sybilled20/assets/160050412/dd1e9abc-ccb8-4784-a87d-ef9e7bc987b2">

<img width="776" alt="Capture d’écran 2024-05-15 à 17 07 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/728cf9c6-c204-4814-96bf-d4d009343314">

  <img width="743" alt="Capture d’écran 2024-05-15 à 17 07 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/0cb776af-45d0-42f7-b8b8-277dd44e19a7">
<img width="784" alt="Capture d’écran 2024-05-15 à 17 07 17" src="https://github.com/ultratwo/sybilled20/assets/160050412/db17d8a2-11d7-4316-9548-d901e2001fd0">

<img width="740" alt="Capture d’écran 2024-05-15 à 17 07 27" src="https://github.com/ultratwo/sybilled20/assets/160050412/b8209cf7-9b40-4405-8701-5e8551142b40">

<img width="757" alt="Capture d’écran 2024-05-15 à 17 07 32" src="https://github.com/ultratwo/sybilled20/assets/160050412/7bd9fec1-36e7-4eda-adaf-2a61b135601c">

<img width="755" alt="Capture d’écran 2024-05-15 à 17 07 37" src="https://github.com/ultratwo/sybilled20/assets/160050412/69cc2282-daca-4a3d-9b25-89cebfcceba6">

<img width="766" alt="Capture d’écran 2024-05-15 à 17 07 41" src="https://github.com/ultratwo/sybilled20/assets/160050412/82d3b880-2a36-4bee-b8c0-0d6faa706314">
<img width="754" alt="Capture d’écran 2024-05-15 à 17 07 47" src="https://github.com/ultratwo/sybilled20/assets/160050412/cd71475c-773b-4e42-9f1e-dd8ab86cc0b9">

</details>

Cluster + same CEX deposit address + same on-chain activity.

## CLUSTER 9


The first 11 addresses of the cluster share the same Binance deposit address 0xfA4C348598366DD76893517196F997100Ec453b4. The rest are linked to numerous addresses of the cluster, multiple times.


```
0x9ea3153784b4e5305bf37bcad64adb35bda4049b
0xecba4ba5c81b878993f1710daa6b913d5f13912d
0x1d27b844cadb9a35285472fd05b5005157749187
0x7b51a40c0ef296eac9ec3196bf3511445151326a
0x837f4759b2727454833f4aabade70a47970af352
0xec6bc36a9e71c50d279d8516571cd55733cd9cda
0xc1d1f09741dbcd0b4ff0b8c37b7c020910adea7c
0x57039b89d2Faac39370A19fe5b1cD5E43539b39b
0x4ac4f44ca6153586212710bA30cEDA55517B374B
0x0E90de187864960C8De6a103Fd8bAb6758530b6E
0xC2dB5e5ADc96834b2Cb8C449e6e5DE57F5231f9b
0xe6943b595c588738727bc7b040dd60f7e586d0cd
0xfb1865f4afbde18f12b77669f586d491ebdc7a23
0xd272fef1871a3b040ddce6605aa8c1d28f6225ef
0xffc0d596ea91403d6c36a8203dbf86b05184893f
0x707870ddcd92ef6dc54bceb946cc3d91c5a03da9
0x8d7849848a6485bb490a5f5f5e18f5ba36fb192a
0x00f584c8507ebc4e4600adbe0e8684bfcc87bcab
0x82ac359d1a218e843a223a741dd154a82cf4e88a
0x4dc8bae868a28d56414a3b5405abe1e0817c5bea
0x18971df836ec5a8f9c49bb4dec560623af70b5da
0x6e75cf0f3c3f0b1895e6aebaec1c08298f9544c9
0x56c2a24c21d42d173d1f75dc28220ee74e76ff0d
0x738fdc2eb099de4b42d50861ed717deece61f2be
0x321edf73dd11b14fdb7bc771b2168371c5ecfc34
0x17660eed0663b962926d70598cbfa02303cdcbcc
0xa3c12dfc26d9e3d4413d9771eb4e3ae62bde39cc
0x60e19800d62d4ef0c210aac0172cf109c2e76fb5
0x19c64d404b2ede3129be07e5cd7e22dfa782d1db
0xc84865662b45acb43df102bef1777d0198484b7d
0x99b6b414d0bdd441ab6ceaecec819c5a06f7c76f
0xbbabc9bfac36bbe6625ae03c91a4115703676c47
0x816e00a3493761511fb03c63b2aaed01686ce936
0x90117a73bbe1845b4eaaf63c7a731ca579745f53
0x6b7b0add6bd5f545613a39ba230a2c973508320a
0xf1da0d8a98be411b9ce9b255c74ac117960bc942
0x26a807a0ef233ffbae4988d2985035c6e809499c
0x5539f943e41a80852036c377d2f4bca1fe798a1e
0x7918d3523c36247eafda6cf9df0160d3a54c127d
0xdab28ee0333bb715042b0fed54123cc172e2e228
0x97f9c52d4354cdb31fd63a24b140e390c6149b0e
0xfc9c9f2a17dae0dfcc7483340160e1e28073c4cd
0x28d34f3ce948d41ad45137eb993fd83948f1f3f0
0xbca0d15cd9d71466c03489993c6ddbf3172d9f2c
0xbcdb63fa8b53549ec57ccc6fad541480d4fceb9f
```



<img width="508" alt="Capture d’écran 2024-05-15 à 23 50 59" src="https://github.com/ultratwo/sybilled20/assets/160050412/e2fa51be-8b20-4807-91d4-85bb3cd06d45">




The addresses have the same on-chain activity. Their L0 is the same, probably due to a script. For example, their latest L0 interaction always is the same: Stargate transaction 3 months ago from BSC, and Holograph transaction 4 months ago from Optimism, for every address. The same patterns happen over and over.


<details>

<img width="898" alt="Capture d’écran 2024-05-15 à 23 52 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/509f9c0a-8aec-462e-aa36-04b39870a7d8">

<img width="894" alt="Capture d’écran 2024-05-15 à 23 52 22" src="https://github.com/ultratwo/sybilled20/assets/160050412/2db40593-de8f-4f02-8c61-0ebfb916e6ea">

<img width="899" alt="Capture d’écran 2024-05-15 à 23 52 28" src="https://github.com/ultratwo/sybilled20/assets/160050412/ed2a1f46-85e5-42ef-a0b7-3da01ca60acb">
<img width="890" alt="Capture d’écran 2024-05-15 à 23 53 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/8b71711e-cd6d-4f2d-9904-e758d4d888dc">


<img width="903" alt="Capture d’écran 2024-05-15 à 23 52 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/e5fe43b3-6207-46b7-a1e7-f88eec70561c">



<img width="925" alt="Capture d’écran 2024-05-15 à 23 52 42" src="https://github.com/ultratwo/sybilled20/assets/160050412/18a29097-e96b-4ec0-a946-4784c7e97b7b">


<img width="895" alt="Capture d’écran 2024-05-15 à 23 52 47" src="https://github.com/ultratwo/sybilled20/assets/160050412/755a5488-84b4-477c-8c3a-733df7102ac5">



<img width="880" alt="Capture d’écran 2024-05-15 à 23 52 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/70a644fc-7bd8-437e-ba15-f2d9130623ed">


<img width="880" alt="Capture d’écran 2024-05-15 à 23 53 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/d50d9b81-6d3a-4b1b-bbdd-c669dd05b70a">



<img width="895" alt="Capture d’écran 2024-05-15 à 23 53 34" src="https://github.com/ultratwo/sybilled20/assets/160050412/313ecb22-e1b0-4a62-8008-89722bcf12c1">



<img width="907" alt="Capture d’écran 2024-05-15 à 23 53 40" src="https://github.com/ultratwo/sybilled20/assets/160050412/3719f221-1821-48dd-aafe-d25215725686">
<img width="880" alt="Capture d’écran 2024-05-15 à 23 53 45" src="https://github.com/ultratwo/sybilled20/assets/160050412/2ded54e4-a842-47aa-9cdd-99e7e29a3269">

etc...
  
</details>

Cluster + same CEX deposit address + same exact pattern. There's no doubt this is a sybil cluster.



## CLUSTER 10


The first 12 addresses of the cluster share the same OKX deposit address 0xA02fB2b415BF6FD935121BA19DeB6D6FCE5e98aB. The rest are linked to numerous addresses of the cluster, multiple times.

```
0xa9442304a2d3bccf0af7515636b849989f5579a7
0x8223e79dbdfeb764acdc3e71dcf3ad41bb3c6778
0x78b76de2820af944f3acc7d97a4317217979341c
0x826239d2631177eef34cf0e11d5138373c19f30f
0xd1d23178f40827f6d18a63124a2a3706e459cbf7
0xd6aa58dff7565f2c4b46a523c273bd6873094fcd
0x3a96ab405d53507ce6e5de43a9030ecd33ea80b7
0x9809b86eeec676b4c003ee2eb5276f6b915d1e1f
0x907afbb088fa96ed75e5091478d33c6f5547b1aa
0x244522c5482c0ba35712826e43d99d16d2c2b22e
0x65d8f51b936133b3a486f34e290d7a9790352622
0xbfa8e63ff38033dcf7c450a4d40aff055357ccf5
0xe22f7ab8cb84d9e02f3631364408687ff0b70479
0x71b606dadbbd050dea735ffab6fa2d4eec8c637e
0x249ae9c7cc0dfc462a93f740f20e8ad42e835e3b
0xa10abaa65d418a010b0436c1c19a637b8a612b05
0x86c113a81bce1472287484fb2e75b66900e8b98b
0xbcdb6595593161b446b36566f5cf1c91b963538b
0xc86df7aead4e2870cc4b61bb76e445672c9c5d10
0x106597e5f8303cbe58ae1af8433795cb71f90287
0x4c9173533d9f8d0b507db2c581b4df979d08d06a
0xcfc24df80ff9785814cafcdefafa7c0f12132486
0x2d80b41f59f10a0426bae33440f73c6201c2cf4e
0x7802bbbc1a377c9cd2d31a7eae61b1ee93a7d52c
0x211e988019e97700bb95687162eb210c989e093c
0xc2510a9fc2c341973243240b7d3da3dc37ef0a62
```

<img width="555" alt="Capture d’écran 2024-05-15 à 17 16 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/e5846048-b11f-4467-a195-4b2e3518c6ca">


The addresses have the same-on chain activity. For example, their latest L0 interaction all follow the same pattern (probably a script). They interact with the same DAPPS from the same blockchains in the same timespans.


<details>

<img width="892" alt="Capture d’écran 2024-05-15 à 17 18 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/289253a6-585f-46c3-851d-2538c691c514">

<img width="891" alt="Capture d’écran 2024-05-15 à 17 18 28" src="https://github.com/ultratwo/sybilled20/assets/160050412/b92f84c7-9a55-45cf-8f5b-79ff5fb07b4c">



<img width="888" alt="Capture d’écran 2024-05-15 à 17 18 40" src="https://github.com/ultratwo/sybilled20/assets/160050412/5be1d6f2-451c-4c52-a656-6200006766e5">


<img width="888" alt="Capture d’écran 2024-05-15 à 17 18 47" src="https://github.com/ultratwo/sybilled20/assets/160050412/a16f7475-b8c8-47a7-895a-23b4826927a2">


<img width="899" alt="Capture d’écran 2024-05-15 à 17 19 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/98ad3e5d-20d1-45f5-9c64-bb9fe29c9e25">


<img width="895" alt="Capture d’écran 2024-05-15 à 17 19 14" src="https://github.com/ultratwo/sybilled20/assets/160050412/ca357f05-6de4-42c7-a516-6f968fa2f218">

<img width="921" alt="Capture d’écran 2024-05-15 à 17 19 21" src="https://github.com/ultratwo/sybilled20/assets/160050412/a73bc8bb-03da-4e3a-b1c6-f1b7566bc813">



  
</details>

For example, the addresses used the Aptos Bridge from Arbitrum in a 48 hours timespans. 

<details>
<img width="777" alt="Capture d’écran 2024-05-15 à 17 21 31" src="https://github.com/ultratwo/sybilled20/assets/160050412/92cff6e6-f17e-41ed-b086-f97319ca1cda">
https://arbiscan.io/tx/0x38c46e26f679d5b0042b6c8bbc145b57bc0a640fd4ac83c18be6feb8061e83e5

<img width="786" alt="Capture d’écran 2024-05-15 à 17 21 50" src="https://github.com/ultratwo/sybilled20/assets/160050412/68e40bd9-7529-4d7d-b94c-290c04b59c9a">
https://arbiscan.io/tx/0xc013133dccf26d9c0be6d63ab061fde177dc2feba5d4488431fc27c4cd4a5dfa


<img width="729" alt="Capture d’écran 2024-05-15 à 17 22 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/4f5ac84e-e0ff-49d3-8c8f-ba827ef4ad29">
https://arbiscan.io/tx/0xebe350e27caeb01949dcee43880d810a7a8e79181832a66624fdac04eff766c2



<img width="799" alt="Capture d’écran 2024-05-15 à 17 22 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/f32fd443-8e69-4fc4-a088-3bf03393f195">

https://arbiscan.io/tx/0x42f4efd2b91040a5babf71fcea162a5394bce4c6d168035a8acb4219d7957799


<img width="770" alt="Capture d’écran 2024-05-15 à 17 22 24" src="https://github.com/ultratwo/sybilled20/assets/160050412/6938ccf8-bb8d-42a6-a3f4-f3fe1f4e62de">
https://arbiscan.io/tx/0xc3cacbc89f8829c715817d1374805e6bac7cb7245359ca0bf50316f3d680946d



<img width="785" alt="Capture d’écran 2024-05-15 à 17 22 37" src="https://github.com/ultratwo/sybilled20/assets/160050412/1b2a3ff2-773b-4339-9f96-ab07c7325172">
https://arbiscan.io/tx/0x53bf1cb36dce59652bb559e0c9d16a1dc4287720ba351288fbab039390ef8804

<img width="782" alt="Capture d’écran 2024-05-15 à 17 22 54" src="https://github.com/ultratwo/sybilled20/assets/160050412/0c4dfcab-1728-4820-817a-aaccb3206f18">

https://arbiscan.io/tx/0x918e93dde0becce836046e0c13ebf4978b2222cb2906e8eff9aff1092ed7547b
<img width="797" alt="Capture d’écran 2024-05-15 à 17 23 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/e1592714-3f05-4b54-868b-d733319b621f">
https://arbiscan.io/tx/0xe21dc36c46ed33c5a9480b0d8763d332b20aae8503496f82ece6bd9837c9cbf3
</details>


This can go on and on (Holograph tx for example). Cluster + same CEX deposit address + same on-chain activity.




## CLUSTER 11

The first 9 addresses of the cluster share the same OKX deposit address 0xA5205183812c78c497004EeF93690be86B642cC0. The rest are linked to numerous addresses of the cluster, multiple times.


```
0xbe556e16aef7ed67ff548d8d3da7022a3358f33e
0xaa1d1927fce951bed3d19d556fd1d3b1fe83c99f
0x457f79280dd54afbe49b8fb7f0ee38ffa77baa52
0x1a8fc88f0ffbde449201ef162e41baf5b68cdda0
0xccd70cc27aeb999920b760b0255741de3c7d6b2b
0x610a490da17f804be43534e85d31fd7fde7f5d73
0x4682437891f03267dbf752ab9893096ec18e1e81
0xe28fc6fc50129aa5e2aa0312d88c32d36f2269f4
0x5e5261f15bf1a3ef6c3a15e54580e30fae4ed01a
0x334b35d0d85a63e491170448d59c1b037e9f1534
0x10da836f9ca3944e5d47670d703c234561f35347
0x95ca8e1987fff0282530f1be5a83bd41e8316943
0x03e3cf9dfa189ec6c5b8fd21d063eb6de19e0d95
0x72d37a9d21897373a1bcfff792c49e48cf6a223d
0xfaed7b7a54f90c5526e78e8c98d4c3fd9e92cf6c
0x8bb3d8c2d642958c131cf1376fd8da564e884f12
0x594c08365dcbec8f31bb560ab01048f229498a75
0x46c6b415a5652b4b9c57f62c77fdd465d3edbc1e
0x8c7df16a7511b9b79134597bf19677279d405d6f
0xa8bf53e2affba978b62bc0321f400b12b4db583a
```

<img width="609" alt="Capture d’écran 2024-05-15 à 17 45 12" src="https://github.com/ultratwo/sybilled20/assets/160050412/7cb6f21c-698b-451c-b92d-fb18a4d6d1f3">


 
The addresses have the same on-chain activity. For example, they all locked <10$ worth of STG on Stargate on Arbitrum in the same timespan.

<details>

<img width="752" alt="Capture d’écran 2024-05-15 à 17 47 57" src="https://github.com/ultratwo/sybilled20/assets/160050412/89e7ca46-4333-47f5-94e7-dfab080d815b">
https://arbiscan.io/tx/0x3bf04311e76f445085e1e8a4dab1816ba8b3513369ee9a0e460e77f13c91b946

<img width="773" alt="Capture d’écran 2024-05-15 à 17 48 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/fea88253-0a1a-4593-a1cb-9047a20f71df">
https://arbiscan.io/tx/0xffc8f6431f6e6bd6313b3f1c9225f1d4bb84bd717dbdce4983a3ef17d6ffc59d
  <img width="752" alt="Capture d’écran 2024-05-15 à 17 48 19" src="https://github.com/ultratwo/sybilled20/assets/160050412/cdb65f95-46c0-4572-9d7d-5791d3203570">
  https://arbiscan.io/tx/0xf0009a268becb9b0716fbbd0342a0594b5c80356a3ca45ecc2e1f8deab4743a5
<img width="765" alt="Capture d’écran 2024-05-15 à 17 48 26" src="https://github.com/ultratwo/sybilled20/assets/160050412/ef029e0b-9d5e-4b6d-a25d-5fb13918d7d7">
https://arbiscan.io/tx/0xcafffa16cf173f90b4d2fe8fc0183c6bbe658a1784ed73bf6996beaa607f08ac

<img width="766" alt="Capture d’écran 2024-05-15 à 17 48 42" src="https://github.com/ultratwo/sybilled20/assets/160050412/835afc60-87bc-4cbf-9cf4-bdb6f634fe2c">
https://arbiscan.io/tx/0x70b3abb8cdfcf07dc9c761f56ec788488c9276807a5358849a7137e241d38610
<img width="748" alt="Capture d’écran 2024-05-15 à 17 48 50" src="https://github.com/ultratwo/sybilled20/assets/160050412/24cb9886-3592-449c-a54d-da9b78e8747d">
https://arbiscan.io/tx/0xf6e6bbae5bcbc76c40fab6f1685f0ee414546a4d7cfb0de35b273345351c9f68
<img width="763" alt="Capture d’écran 2024-05-15 à 17 48 57" src="https://github.com/ultratwo/sybilled20/assets/160050412/38de0e5b-2f75-404c-b178-a1fa30d9a98c">
https://arbiscan.io/tx/0x000ef18a896c3c47c22eda4c6e16c60fdb101e8c6893d357510e9f9fd441b47a

<img width="793" alt="Capture d’écran 2024-05-15 à 17 49 03" src="https://github.com/ultratwo/sybilled20/assets/160050412/8e404c70-8903-4555-a068-3ed0e3184a4f">
https://arbiscan.io/tx/0xfdeb53f08d2bc34b35d2f826e5b46d04849a6575172d8f126227a12bcf2a1a67

</details>


This can go on and on with other examples. Cluster + same CEX deposit address + same on-chain activity.

## CLUSTER 12





All the addresses of the cluster share the same Binance deposit address 0x77f64CBb63149aF19c1C9BCd1F9833dAca4bd224. 

```
0x089530e865a9ca48507916843dd932481d9c2019
0xb48dd89ee1d30320e9a1fc0c6ab8f12ee3762e92
0x6b0b236f8433f0462f5dc4377b9e9a99c2c36499
0x952be8134322ed1ece740280f6ef2b21de9e2d1f
0x32b65ee3722ef6f4a8d04611fcc6df52f433504d
0x5fa1e7b779a06544fffff825b10b736a056a20d6
0xd751b975468d97767cf6f827466e3eee08a834f9
0x6c25880fa40828782059d98eceed91075532bb47
0x1f428097d0fda51f4e8165d59c3306cafabb971a
0xb07809c4fe970dbe2b487067366af83f3c3fa840
0xd4600db5c4db3d77b3ba356ae78b7d505748bd04
0x37083acc364a8ebb2799e8dad5fec5dc38cad00d
0xd09184efefdbb0fe03197b92bc18c47bc57cd5c1
0x6853351321914042ccc677b1df9be1e61acbe10b
0xb73b0329ad7e7559f58e77af38857a30fea30774
0x27c5e0beb41eb8d02e845eeb2b7cbb4f253aa1c0
0xacaee28ce71f2e6a11f4c0e25065894147de8882
0x03a98c3297b4d16dfd61e619cde806d638029032
0x8649e075a5c6f3c5a427abf99cdc03b291dd7dc6
0x878f04888c26fcf3b5e9fc9b13e82534eb29cfc8
0x4eaa300ce3c6e482005de55df8b823905a3e9977
0xa9ea8473434a4077af18ed517159c37adb26bb1c
0xe9139bb23f1c550dbc7c1b7b56194a5ca3c83256
0x7d2fd766d894eae2c25a8c23515864985ee0d354
0x55cea0088250eee4e503f22898aa229af92e9bb1
0x00737160876a4aaa57afa84834b04d58722f95d6
0x29464a561e4c78a5a5bdb5b36ca5e2a3957d7a94
0xb641e6bf0dd37b9a2b1865aac55846deaec7418d
0xdc7c76ac9e1d740a1909e5d481658842ce8a8ae5
0x0422f525da3560980572b1101479ea7ed3462c69
```




<img width="479" alt="Capture d’écran 2024-05-18 à 00 52 33" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/98ae7479-672e-4479-b676-5c32f9c8c5dd">

The addresses have similar on-chain activity. They all have similar LZ Age.

<img width="1108" alt="Capture d’écran 2024-05-18 à 00 53 47" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/79ea24df-d29e-4d99-9485-8bcdc0105ec3">

<img width="1113" alt="Capture d’écran 2024-05-18 à 00 53 59" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/323dc2ad-36ee-4624-81ab-4437feec15a7">


The addresses execute similar transaction at the same time to farm airdrop accross planty wallets. For example, they spammed the Harmony back and forth with similar amounts during the same timespan.


<details>

<img width="632" alt="Capture d’écran 2024-05-18 à 00 58 45" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/a8ffe6cc-9231-4bcf-ad99-df1dd96da89e">


<img width="634" alt="Capture d’écran 2024-05-18 à 00 58 53" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/30543613-d264-4d83-8c3a-a9d9e2099ff0">


<img width="633" alt="Capture d’écran 2024-05-18 à 00 59 00" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/83cf5bd0-b85f-436e-a0a8-b1a86ea307a1">

<img width="610" alt="Capture d’écran 2024-05-18 à 00 59 06" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/94cd9fec-665e-4f84-9714-827b7ac45977">
<img width="614" alt="Capture d’écran 2024-05-18 à 00 59 35" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/527806b3-3b78-42f5-bcea-274e404c08f8">


<img width="649" alt="Capture d’écran 2024-05-18 à 00 59 14" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/d2c886c9-3b17-4788-9907-278dc0cbe114">

<img width="641" alt="Capture d’écran 2024-05-18 à 00 59 21" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/f151a48a-c0dc-49b9-a37d-7af0c44948d6">

  <img width="635" alt="Capture d’écran 2024-05-18 à 00 59 28" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/7ae0877e-c658-40b4-8760-2fca5dd6705a">

</details>

This is a low quality sybil operation.





## CLUSTER 13



The first 11 addresses of the cluster share the same Binance deposit address 0x5e50CeaDA619DD2A8c8AD33BC563c36d18A223CF.  The rest are linked to numerous addresses of the cluster, multiple times.






```
0x126cfe939f67d8397b4681bd76a663738e67a8ca
0x8c02f56430395dfe3c15adde63f626249484b68d
0x1cda196a5eff21dc0452fcb5bdffe76f2529290f
0xe534897ed81c97466e9127124cf19a39558322b4
0x2361b262dd2c64e1ffcecea208382532191906df
0x5d3d9f847fd97ec6a324403f7adbf5d8f3ec1920
0x6c51fbb94d683f74b8e83084f4fec40299759ec0
0x1d6068138d02423520a2c2b772f48f52c07dc18d
0xb5c0caa6d0a712153b351e82544b2f6252f6ab2d
0x12f5c0b1d15dc7bba4a41dda1a86f408b8388a1a
0xd439be8b8ba0d3ee6dc476966cbf88059880f76f
0x1e884550b686a03095758f8353c21629ed0a5e79
0x434d6c0728ad1ccf6786bac7ed10fb322f14dc8f
0x1facb89398e5f2ce3343db166f4c60bce3b1c874
0x1807ad77c573845c50cf002166b716714aa6c376
0xca6f69fe567ae03c5030e10e219c2bc21a745abf
0xbd40bd86803ee8ae5cb824c597878135eebe591d
0x68a1b085007b078ce4b6b9af23cbfdba3835e0ab
0x91b7a474c1975af88b8c815cfea57aad7cf6415e
0x93166ccfa055112c1841eb0e78b75bdd44718774
0x3ad80a07687be48f1ad5fea7fa30aaa409cf49c7
0x3707387f12a3727fb0f4506967aaefc5fc1e14b7
0x17451c0309a0c5cab5fd1f46193cf9faeea9bba0
0x18edc3479d56269661454a4ea4185360cd123c30
0x77d91b054785a329f320c10ac1c58a2d4699eb74
0x2ce8fa74a1da289003e9f93084a3728ec5a56042
0xd545e0dcfd4e93d0af39c6e31193614b84eff385
0x371409a8166a6db2f6fb5e7d7722953294517d33
0x23604d6df9df6365e2e2de97331160ce496501db
0x22f6cb0639d418459e5589d7208045e1e4e70804
0x48fa4fc578274cd864bf456d56c68bafbc026f0d
0x9a6e3520d76617d9a7eac62e3bdd08e917566703
0xec7f1762505f753030c8bab53ed6991a473089ed
0xc6fa530e16f0f5cbf57cbff6e5e7a7d2613e398a
0xac20b8751a75ba1f72932833cc8a1d9a5ef82e12
0x85d06dc0db6204f5c6227f4f316cabdc4600e7b3
0x6dafead47aac98c80e60d65a5396c17e39961642
0x44fa4f2be10e2fe8bfa8356eecc82f58ac7f147d
0x60066cc206d8bfa6c3064cb7a6fce98c2f660163
```

<img width="436" alt="Capture d’écran 2024-05-18 à 00 23 22" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/ca7ce334-20ba-4108-9f6d-9a14a79d1723">



 
The addresses have similar on-chain activity. They have similar LZ Age, similar unique days/weeks/months, similar number of transactions, similar contract counts etc...



<img width="1095" alt="Capture d’écran 2024-05-18 à 00 25 33" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/45655cdd-ebe3-4a43-ab03-25bf1f5492db">
<img width="1107" alt="Capture d’écran 2024-05-18 à 00 25 41" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/918da649-4b27-4b9c-9b0c-eefc18c5d5cd">




Their L0 activity follow the same pattern. The latest is Aptos Bridge 1 month ago from Arbitrum, some BTC.B transaction from BSC or AVAX, another Aptos bridge transaction from BSC and Merkly Spam from Polygon.
 


<details>


<img width="898" alt="Capture d’écran 2024-05-18 à 00 28 57" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/8659653b-7a09-4f76-8210-fd082ce34a93">

<img width="920" alt="Capture d’écran 2024-05-18 à 00 29 22" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/a0479f53-7420-40f8-a8e2-873cec150d32">


<img width="891" alt="Capture d’écran 2024-05-18 à 00 29 04" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/65996998-d618-40b9-8a7d-0b9e52fb80b1">


<img width="895" alt="Capture d’écran 2024-05-18 à 00 29 10" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/2268de4c-1b25-43ae-89bc-0a988c288f67">
<img width="889" alt="Capture d’écran 2024-05-18 à 00 29 15" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/40e71c4b-96f6-4002-b374-40f2ae55c725">
<img width="918" alt="Capture d’écran 2024-05-18 à 00 29 44" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/de9e289e-b754-445e-b195-30333030e5c7">

<img width="896" alt="Capture d’écran 2024-05-18 à 00 29 37" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/29f6ac60-c9b2-404a-8d91-1c50b61fa43a">

<img width="906" alt="Capture d’écran 2024-05-18 à 00 29 30" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/7c57a373-1e65-4e88-941e-b5ed930e0432">

etc...
  
</details>


The addresses of the cluster execute the same transaction at the same time to farm airdrops, probably the result of a script. For example, they staked 2 STG on Stargate BSC the same day( 12 hours timespan).

<details>


<img width="636" alt="Capture d’écran 2024-05-18 à 00 35 09" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/4c6bd971-817f-4ca0-b74d-5eb03b6f7b53">
https://bscscan.com/tx/0x4a063fd3946be5761741d10dcd3a3e00bf68538cac6fc61d893cffee23b6d66a


<img width="685" alt="Capture d’écran 2024-05-18 à 00 35 15" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/9fd92e1f-a9c3-4abb-a114-72596977c30f">
https://bscscan.com/tx/0xe37bbf0c3c732b5be7e1644a644edd950e36a293908dbe32d5a108cf5e6102bb

<img width="640" alt="Capture d’écran 2024-05-18 à 00 35 21" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/baddf121-032b-4a3d-949b-7e4bb765800e">
https://bscscan.com/tx/0x5875d8be25ad26a146c1b63f6d362da7312c0b37d8ac3063bd3b4873e4a2035a
<img width="637" alt="Capture d’écran 2024-05-18 à 00 35 33" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/e9725151-1e5b-45c0-9dc7-1ff111b962e5">

https://bscscan.com/tx/0xefb8c314e7b49effe4dba21d36f6a5cc5f7c3e6e2fbb724ee4af7f2d166eb40c


<img width="664" alt="Capture d’écran 2024-05-18 à 00 35 45" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/7158c57a-ee5a-4084-9b20-4642b759045b">
https://bscscan.com/tx/0x514281c1d50f2c7a1e701d19e2e7097645ebe032ab8bcffaf8abc273458badf9


<img width="677" alt="Capture d’écran 2024-05-18 à 00 35 53" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/f88d4cbb-18a3-4792-9f62-faad7ce5940c">
https://bscscan.com/tx/0x3379474ccc6a1b166cb94baf1002bd9ac8d93e84497e0115dc8d87e847c62ed6

<img width="653" alt="Capture d’écran 2024-05-18 à 00 36 03" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/eb48e254-58be-4463-a243-4240e90af658">
https://bscscan.com/tx/0x0ce11d68f137f99f260727dd3b6094258a9ff7b1623bd495d2a1ef01f95a1088
<img width="646" alt="Capture d’écran 2024-05-18 à 00 36 11" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/acccbaa3-50f4-47a0-b032-aeb693ecd881">
https://bscscan.com/tx/0xb7f155ae87d40a5b780c11f0d755a86ffd5d3817879052bc8067d7e40ab9d88d


<img width="649" alt="Capture d’écran 2024-05-18 à 00 37 16" src="https://github.com/ultratwo/sybil-report-continuation/assets/160050412/e6d86172-dd93-4275-b9e0-c0cd1578451c">
https://bscscan.com/tx/0x7f51e2ca83c6c5cb6b8be42ba0ffb9e5760793b90620db3fa9d51e4f9117cbb6
etc...
</details>


Cluster + same CEX address + same activity accross +20 wallets to farm airdrop. This is without a doubt a sybil cluster.




## CLUSTER 14

The first 12 addresses of the cluster share the same Binance deposit address 0xD60221372dCB087CF70a9B19F0C3E6583A6d1614. The rest are linked to numerous addresses of the cluster, multiple times.


```
0xc0ad0a8a9009e92a34a10e8b99ba48b4dfa3ff90
0x08c68e2cea3ec60508c23cc96efc71e70164a7ab
0x1625a07d88f600877ce0695f36874f32431e1111
0x2ecb409ec3cbbacdf073ca5d6e2dee5b7e1f0000
0x9aeb20df6e3dec0e4e72d6155995edabe319e7b6
0x47a06551815b18adc6d0216a2fca84b342907e1a
0xb689490f72d1bd3dc86c65e1c9a53fbd35c2c0a3
0x1add1758b593952e6e34e6a436a02a79a9dd9e9d
0xceebed28e1e927ac6da488bfe5e11c4089272fd1
0x26aa9cbf025fb9938056476b77fe7c5c374c2222
0x37179dff48bc792497dafb2cd575f82333801278
0x4f4e13b91c31c6db330e1c375b9c6f86eaea411e
0x0aff928f68f0fb75409417196986e1be9ce33333
0x29b40aa7b0d30230ee01ed8c47683c5b9ac0d793
0x4cb091f7a6efbe810da4bd51f7f6cee6dc10f2b0
0xa35468b156b4e0654e8c002dc19e50e4af3a5555
0x98b6e90d3ffad367436aaa32fd2b6577ff0c6666
0x03d4970a4eafa16482043872e4f2ed9129a7e4b9
0x02f9b9ae100631cd96800bb8863f6fe985698848
0xfe3fd87ea997fbeac80b355f15831dd3c78cdbd4
0x0a7851b65460fa2f7048001188507c1c07a31314
0x80b7948ea2575b16e5431d07a6a027c0087e4444
0xe07b8c3f4e4dc5b8be3c64339bcb952d2d6d5a8c
0x0b233e7044f495e6bfbd3711434e414344a5ff8a
0xb38b20db61be73d38c64b1d7b9a196786fab5f10
0xee5ad4e4b39843bb228a88816942fab8ceb08888
0x86fb8b44c9e3e42bcd6485e014bfff50a5a05e32
0x3f5aa1f4a0b9080cca3bc4d7874781d6485094d2
0x4b1645f0eb1c388b910faee1f46e90ebb3b1b3fb
0x9351f29ee6dc7ebe2886eb544967dc4508e81d9e
0x87d1f1e5391d0f280480f2f8fd2319bae8f69999
0x867f519504db337b9092085fa23670684f42b5fa
0x2f6122979b2f5d4dcafe942532e01ccfe59bc071
0xac708c15091a22aa48b50c7dfb83c2ff63ec1314
0x83a67ca0a5dd8778bfa86a2b0a1bb13d44a08848
0x1742a32d1bcf66899aa3b225e465a5b5ee6e7777
0x9ac56c1107042ee95b826a816a671312316b8868
```

<img width="640" alt="Capture d’écran 2024-05-15 à 20 57 58" src="https://github.com/ultratwo/sybilled20/assets/160050412/de7f4fc3-14cd-464d-8100-990e5833113a">

The addresses of the cluster have the same activity on-chain. Every single address have the same L0 activity following two different pattern.

Either their latest transactions are Stakestone 4 days ago and CoreDAO spamming, or Orderly 4 days ago and GasZip+Stragate before that.

Pattern A

<details>
  
<img width="905" alt="Capture d’écran 2024-05-15 à 20 48 18" src="https://github.com/ultratwo/sybilled20/assets/160050412/400cb8f2-3415-4104-a679-17a99327021e">

<img width="906" alt="Capture d’écran 2024-05-15 à 20 48 29" src="https://github.com/ultratwo/sybilled20/assets/160050412/02e5ddeb-c31d-4382-a6d1-e9cf80a48d37">

<img width="902" alt="Capture d’écran 2024-05-15 à 20 48 53" src="https://github.com/ultratwo/sybilled20/assets/160050412/f93e0256-6229-42df-9d0d-31866762a18e">

  <img width="900" alt="Capture d’écran 2024-05-15 à 20 48 37" src="https://github.com/ultratwo/sybilled20/assets/160050412/41c1f755-2ed1-402b-af82-197e249811be">
<img width="903" alt="Capture d’écran 2024-05-15 à 20 48 44" src="https://github.com/ultratwo/sybilled20/assets/160050412/30b6117c-9e4e-4cea-8d0a-ecd506e383a8">


Pattern B 

<details>

<img width="899" alt="Capture d’écran 2024-05-15 à 20 49 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/f0b94c09-4e78-4554-a351-87377f91becd">

<img width="887" alt="Capture d’écran 2024-05-15 à 20 49 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/23139ee3-1309-41d6-ba80-9160bc28e23d">

<img width="898" alt="Capture d’écran 2024-05-15 à 20 49 27" src="https://github.com/ultratwo/sybilled20/assets/160050412/0ea16211-f5ae-455d-880e-3a0fc82aa58c">

<img width="890" alt="Capture d’écran 2024-05-15 à 20 49 33" src="https://github.com/ultratwo/sybilled20/assets/160050412/294ac268-35fa-482c-a3eb-91d5daf253da">

<img width="898" alt="Capture d’écran 2024-05-15 à 20 49 21" src="https://github.com/ultratwo/sybilled20/assets/160050412/50acc555-a36a-4f25-a51b-904d2a76a96e">

<img width="895" alt="Capture d’écran 2024-05-15 à 20 49 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/b97c0eec-80f5-4c47-a70d-bef53236b479">

<img width="891" alt="Capture d’écran 2024-05-15 à 20 49 40" src="https://github.com/ultratwo/sybilled20/assets/160050412/4108fa48-9b4d-466d-bc3b-32354c0538a1">

<img width="932" alt="Capture d’écran 2024-05-15 à 20 49 53" src="https://github.com/ultratwo/sybilled20/assets/160050412/55c46d76-0cb5-485b-8c72-17f6946a31d4">

<img width="901" alt="Capture d’écran 2024-05-15 à 20 49 59" src="https://github.com/ultratwo/sybilled20/assets/160050412/b050e676-39b5-47a2-8fdb-dc726b9f37cd">
<img width="869" alt="Capture d’écran 2024-05-15 à 20 50 05" src="https://github.com/ultratwo/sybilled20/assets/160050412/587729eb-6ef7-4c9f-b4f4-f47e84b986ec">
<img width="889" alt="Capture d’écran 2024-05-15 à 20 50 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/7e9778df-a678-41df-98f6-d7c87d6aa678">

etc...
  
</details>

Considerating the exact same pattern followed by the addresses, the cluster, and the CEX deposit address they share, they're no doubt this is a sybil cluster probably run by scripts.


</details>




## CLUSTER 15


The first 8 addresses of the cluster share the same Kucoin deposit address 0xa588177A9b07f47eFB29E32EC1931925fFcACfAb. The rest are linked to numerous addresses of the cluster, multiple times.



```
0x49c8c6301fe4db765205daa67091a02bc4698220
0x6fdef7d6ad252b5e5325fae52ac5d266c21ae58a
0x49a771f8cffc3790f5beee9296bf3547b9afa192
0x05cab93823349d1c3bdc8314773996ed196c5965
0x19753610e36fc0d7fa248311838b354d03f3bbe8
0x24c245011e40259ae98615d48c7235fc08acbd02
0xec1cbb72bfbe795d1bba5541a36e2952c58d25c1
0x87fbe40f712f6062ff02971777af4d10bec97bf5
0x5b53eccbc68335859124fdd7cdd655a0a9d76a24
0xfd03c26c1b346e6d75ffe07fdc8adf6944cbcfc5
0x9da0104cb80876857de8f090d39d99f8a814329a
0xe7161f9f3680675378a22ff32afec044d6fa3350
0x722a22952ffaa39492e9cd9555e47a2f779b3821
0x30f7509a36e20da6fcce9ab1b304c6eb40e1ff49
0x86373ce82a847abae543c439ce7706de49d6c7b9
0x9aeeb4016658b1f9b066b2117e751418d2d436b5
0xa3b9c351019d71f332524d67ee948ebc58aa855e
0xbbf8d9be237e66a8a98b176a856fd438b9cfaccd
0x4946c861568f284bb14501226bece9a23256f845
0x86879d5358042ec17369756298076323d7c6b9c1
0x769b55e7fae26ed12997d2dae4592ca01bd25321
0x6b2faf800dc12058105f970c83bfd1976ab0dc54
0x545d674a7166341049ad0ec5c5ab5f8f2da24199
```

<img width="511" alt="Capture d’écran 2024-05-16 à 20 53 30" src="https://github.com/ultratwo/sybilled20/assets/160050412/4a4fb8e0-c92a-481e-8d5e-4b3806da3b46">



The addresses have the same on-chain activity. For example, they all staked 5 STG on Stargate Arbitrum in June 2023.

<details>
<img width="636" alt="Capture d’écran 2024-05-16 à 20 42 01" src="https://github.com/ultratwo/sybilled20/assets/160050412/5d655f85-8292-4471-b56d-bc19e2a83122">
https://arbiscan.io/tx/0x4fd18df2b9f5dac1e575425efe7fd5fc4ce452148db28b38abfaebc56b90bac8
<img width="634" alt="Capture d’écran 2024-05-16 à 20 42 09" src="https://github.com/ultratwo/sybilled20/assets/160050412/8365f64e-1c68-422d-9d47-cbc312e24f7e">
https://arbiscan.io/tx/0x0d112a502cda686b9642609a11b68fca94e954ba4cd13b5addab6163e1581701

<img width="646" alt="Capture d’écran 2024-05-16 à 20 42 22" src="https://github.com/ultratwo/sybilled20/assets/160050412/9e215b7a-4ba8-4ea2-83f0-e15208da2f2b">
https://arbiscan.io/tx/0x797297b09286ae6b8585935ff298c1729f636d9938da293b2f4bbd7eb88e669c




<img width="639" alt="Capture d’écran 2024-05-16 à 20 42 30" src="https://github.com/ultratwo/sybilled20/assets/160050412/d8e1dad0-0500-426e-b2b0-592b49761999">
https://arbiscan.io/tx/0xe54346ce3f6e37c59da8a5dfb500aee7886403bd0af1c68da9da2f378d44d289
<img width="644" alt="Capture d’écran 2024-05-16 à 20 42 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/4b490b61-492f-4bc0-aa6f-ded0750778a1">
https://arbiscan.io/tx/0x340238050d7657f37da5c14ccbb8dadfbe0b06c34a64b635c8d61b9e2e36126f

<img width="645" alt="Capture d’écran 2024-05-16 à 20 42 49" src="https://github.com/ultratwo/sybilled20/assets/160050412/69b4912f-ddc0-4a93-be4b-3eca29f71cc4">
https://arbiscan.io/tx/0x73b9877ffb341add1bd3ba0256a0c19b9f836a66a2052a1e8a57480cb78260ae
<img width="643" alt="Capture d’écran 2024-05-16 à 20 42 57" src="https://github.com/ultratwo/sybilled20/assets/160050412/2298f650-41d4-4a29-965d-f38a962b57e6">
https://arbiscan.io/tx/0x7fc9d3d860dcf5d7a50a9276100661478713aa60e4113f20ea6ffe3076306866
<img width="666" alt="Capture d’écran 2024-05-16 à 20 43 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/693b3d6b-ef9a-464f-86f6-5f7e52c973db">
https://arbiscan.io/tx/0x2b37d7fc0a1955e4a960af52a6bbedadd8160df5743cd359d45d5f2cf41ac4ed
<img width="642" alt="Capture d’écran 2024-05-16 à 20 43 18" src="https://github.com/ultratwo/sybilled20/assets/160050412/c92b9bd3-0f5e-445c-9bed-2afd490ebff3">
https://arbiscan.io/tx/0xf7b3316a6233fbc81ced95d3c4510c5f3fbc2e42c7527424e86445a595688926
<img width="640" alt="Capture d’écran 2024-05-16 à 20 43 26" src="https://github.com/ultratwo/sybilled20/assets/160050412/ddaca41e-be65-46ff-95c4-edc2db956244">
https://arbiscan.io/tx/0x26c8f17d8092cb5b2232181e72d9722782bd006c2bac320c1047ab508c749c13

<img width="648" alt="Capture d’écran 2024-05-16 à 20 43 33" src="https://github.com/ultratwo/sybilled20/assets/160050412/d800cee7-8769-472c-8696-8b2a90d4e576">
https://arbiscan.io/tx/0xe5920ee56f22e1a959b14f2c4ff5269f91d4ed260e6ea412e3589362a1c3c306
<img width="638" alt="Capture d’écran 2024-05-16 à 20 43 44" src="https://github.com/ultratwo/sybilled20/assets/160050412/b514f627-618a-4963-8df6-1045862fddd6">
https://arbiscan.io/tx/0x9a4889baa6dbe4a1a6d76665c1a1e64b11a16af37f810d78aaa864d03581e5f5

<img width="640" alt="Capture d’écran 2024-05-16 à 20 43 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/bd8b16f0-0552-4533-9844-ed8fdb6ec5aa">
https://arbiscan.io/tx/0x181c627b073557bdcd8e8b1a16e3029150424d2857b417469fa47987e89b708d

<img width="637" alt="Capture d’écran 2024-05-16 à 20 44 00" src="https://github.com/ultratwo/sybilled20/assets/160050412/b96560c0-eb3d-4108-bd4d-67fe837cb88d">
https://arbiscan.io/tx/0x0d72d45026c263c69d14d5663ac0a34bd725a8ee15faa34747ba4cbccd4243f2


</details>

Another example, all the addresses have interacted with the Fuse Bridge with similar amounts of ETH the same day (48h timespan)


<details>

<img width="626" alt="Capture d’écran 2024-05-16 à 20 47 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/4658acda-487d-4892-90b3-387e9ec06328">


<img width="634" alt="Capture d’écran 2024-05-16 à 20 47 28" src="https://github.com/ultratwo/sybilled20/assets/160050412/6e3979c2-9522-4c53-bfbd-7e4ff548a560">

<img width="674" alt="Capture d’écran 2024-05-16 à 20 47 41" src="https://github.com/ultratwo/sybilled20/assets/160050412/4ed7c7f0-16c4-4f3f-984e-d8b117a393a5">


<img width="663" alt="Capture d’écran 2024-05-16 à 20 46 53" src="https://github.com/ultratwo/sybilled20/assets/160050412/a106a94e-4891-45c0-aac6-91f7f5ca6856">


<img width="657" alt="Capture d’écran 2024-05-16 à 20 46 59" src="https://github.com/ultratwo/sybilled20/assets/160050412/f10df535-ddd8-4b59-a81c-2d335b29e50a">

<img width="615" alt="Capture d’écran 2024-05-16 à 20 47 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/82b5c20f-fbcb-4575-b7af-6f40c3ba6d32">

<img width="654" alt="Capture d’écran 2024-05-16 à 20 48 00" src="https://github.com/ultratwo/sybilled20/assets/160050412/ae88daa7-740e-4f77-8644-bba2a1f4fcce">

<img width="667" alt="Capture d’écran 2024-05-16 à 20 47 13" src="https://github.com/ultratwo/sybilled20/assets/160050412/4e31ea5d-355f-434a-ba9f-340359f92db3">

<img width="628" alt="Capture d’écran 2024-05-16 à 20 47 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/e548eaca-59af-4c25-b395-49e8e4ba22ef">

  <img width="624" alt="Capture d’écran 2024-05-16 à 20 47 33" src="https://github.com/ultratwo/sybilled20/assets/160050412/ff297fca-4ed9-47a1-a792-c21cddc37d6a">
<img width="650" alt="Capture d’écran 2024-05-16 à 20 48 08" src="https://github.com/ultratwo/sybilled20/assets/160050412/9a9be184-b182-418b-b707-37ad3abde846">


etc...
</details>


Cluster + same CEX deposit address + same transactions are the same time in order to farm airdrop accross +20 wallets.







## CLUSTER 16




The first 7 addresses of the cluster share the same OKX deposit address 0x012Ff1003FB3C56c04Cdd3787Fdc4Dac32025211. 15 additionnal addresses are linked to that cluster and to each other.

```
0x6134434b5d1c8587b366393d1cd8c6e934040792
0x6aaf8396a82d63b9b64c30bac0e3b1f610761fc1
0x491e8223efeee474464c340180e7537f37e7323b
0x2eef6c124b5bd700a6f61aaa76e6bf9dfda7d872
0x64febe3aa4ec971e3ddccc049e1b826a9cec65f6
0xaed787f0452b9179f2639aef0d4d1f4d1b050b8b
0x377cf6d587ea42492a291165588ab61ade14a462
0x9ddacf7338313ad4747ad1c210a24bdcd01753a5
0xd12db29b706dbb5b3de6ad074beadb04013202e5
0xdc4941d8c3b916f44341b81c974d62fd5eaf9aed
0xe4c5a675db392caa662cf5ecf040dd0ecbeb776a
0xe260de735c54647fa44435a0f3617e525e543a00
0x4e2b6bc4526d1fcf452d1dfa17b878a21f464621
0xbe87c39126383e4ddcbe871c62f554bc73d2cd74
0x72322bda23cdbc8504378eb6b72aa1cd29456044
0x6e3bdd5d30d18683c1180d07d0c01bda5dd63fb8
0x85428d02b01c0151d5994ea1d9a246c09d74bdd5
0xa9099548a804b3bc92ac91c7fa8c4c745ee6e49d
0x837a36678101bfde7ebf9dbfff85e02b724b7d34
0xc093820273a4e5496ee03f48afdd412fbc282757
0x7a64ff50a847c6c55e0dca2c25d67775ee9ef7a0
```


<img width="570" alt="Capture d’écran 2024-05-11 à 01 18 55" src="https://github.com/ultratwo/sybil-report/assets/160050412/5ea6e237-629f-45cb-b289-26914f2d5283">




The addresses of the cluster presents similar on-chain activity, indicating the sybil nature of the cluster. For exemple, they have similar amount bridged, number of source&destination chains, LayerZero Age, contract count and uniques days/weeks/months : 

<img width="1015" alt="Capture d’écran 2024-05-11 à 01 34 26" src="https://github.com/ultratwo/sybil-report/assets/160050412/4fd8b9fa-e64f-4aff-a670-5c92c64fa8f9">



Their LayerZero activity is the same. For exemple, most addresses used the same. For exemple, their lastest L0 usage is the same: they used Merkly, Omni X, Defi Kingdom and Angle during the same timespan.

<details>

<img width="941" alt="Capture d’écran 2024-05-11 à 01 37 04" src="https://github.com/ultratwo/sybil-report/assets/160050412/7806966f-8427-46f5-b935-1ddc9b993a8d">

<img width="911" alt="Capture d’écran 2024-05-11 à 01 36 55" src="https://github.com/ultratwo/sybil-report/assets/160050412/eb82c734-a0a7-4c37-850e-c11fdd2ef9d9">

<img width="936" alt="Capture d’écran 2024-05-11 à 01 36 51" src="https://github.com/ultratwo/sybil-report/assets/160050412/cdbb84de-c70a-42a4-9c70-9392883bd2dd">

<img width="924" alt="Capture d’écran 2024-05-11 à 01 37 00" src="https://github.com/ultratwo/sybil-report/assets/160050412/f3104a98-3df5-45fe-bde7-bb7707c6c629">

</details>

They also used to provide to stake to the same L0 products in an effort to farm the airdrop. STG & USDC staking on Stargate Arbitrum, and USDC on Radiant

<details>

<img width="890" alt="Capture d’écran 2024-05-11 à 01 47 57" src="https://github.com/ultratwo/sybil-report/assets/160050412/68276faa-3d2d-4657-81ed-a3dbfca9ffee">

<img width="906" alt="Capture d’écran 2024-05-11 à 01 48 01" src="https://github.com/ultratwo/sybil-report/assets/160050412/849a6982-78c3-486e-bee3-974de33e9178">
<img width="843" alt="Capture d’écran 2024-05-11 à 01 48 15" src="https://github.com/ultratwo/sybil-report/assets/160050412/b7f4f08e-0ff9-4b63-b21c-143d43ec9f83">
<img width="681" alt="Capture d’écran 2024-05-11 à 01 50 27" src="https://github.com/ultratwo/sybil-report/assets/160050412/903c06b4-e253-4ab7-938c-36c8a9f89874">


</details>

Considering the cluster that link all those addresses, the usage of the same CEX deposit address and the same on-chain activity, there is no doubt this is a cluster of Sybil nature.











## CLUSTER 17


The first 8 addresses of the cluster share the same Binance deposit address 0x927633325C304E15E9D15aa143Ff847F054EaD2c. The rest are linked to numerous addresses of the cluster, multiple times.

14 addresses of that cluster were present in Nansen's report and discarded. This is what remains of the cluster, 22 addresses with tiles to blacklisted addresses. Screenshots (arkham) and proofs for on-chain activity may contain discarded addresses, but the argumentation is the same, it's even stronger now that 14 addresses tied to this cluster were declared sybil.



```
0x26db6c2ef0bdabba7d578799a0ac89c1f0d90a4f
0x86f6b58646d98f224d0bdcaef9ec717561e751f9
0xc19ba152d9fa90854ffc51ecb41ec3bbfeb97705
0xde924aa663bfaae0b63191e9843df255889c907f
0x83d0d03f76aa04c8e0eb58d5ad51ebe739be18db
0x602c47c1f13d91c05dfed0f23587020415f0e524
0x3a6e34f3e1ee44f1e4605388815b0b7df783838a
0xf4238bf7d4cba389c7eedbb1eea6bc0fc93c1a47
0xbf85c0c3a93aaa14f0da00c75e117ca6b3b43009
0x7b665f4a8a504c09a7f6931628f8b9c054638bae
0x3a4c18f4cce58895eefe3985d91bff17c1420226
0x7360e2f6eed8244f35b1070f6fe3d10dd20a22f3
0xdb9bfbd9ff49877d691bfe0bc22673b2c1a9f161
0xbed6d14ecced7994bba2c7f9ea210b605380b73f
0xcd1b8644c58d5691e2de12ecc1a740e7ae7a4251
0x1c6ba0fd9fd74fd7dfd04e1d7eb763e4f2faf62a
0xbd05a53ce69a5eb3c3919d90a4817a2ba0a75f10
0x2a17ccee60e0b5642b2e7ff3a5246d7e028e2e9c
0x3fc872c93193f63505f7d710591ff8b75f1b3f70
0x3fdf0c278fb36b1da67971037e212800d54cae7d
0x20ac42a33f2e942b3948eaab51e0acde7370eeec
0xe9c8e840937632ac7eeb01ae3f04695deb5b9781
```







The addresses have the same on-chain activity. They execute the same transaction with similar amounts at the same time to farm multiple airdrop accross +30 wallets. For example, the addresses used the ZkSync Era native bridge with similar amouts the same day (48 days timespan) to farm the Zksync airdrop (same thing with the zksync lite bridge).

<details>

<img width="637" alt="Capture d’écran 2024-05-16 à 23 40 19" src="https://github.com/ultratwo/sybilled20/assets/160050412/7a78de0f-da70-4ccc-84a2-2afcba495b0d">
https://etherscan.io/tx/0x1eb20eb7e50709318fad9083aabf0d68a26729bf2a23ddcc894f6607b7b43375

<img width="646" alt="Capture d’écran 2024-05-16 à 23 40 26" src="https://github.com/ultratwo/sybilled20/assets/160050412/9351ce35-e176-41fd-bd9d-a159bd8cd4bc">
https://etherscan.io/tx/0x0bcffd6e70009bc2274d73474be2fdb9e1eb43ed99d4f9385fdc44923a438ae8

<img width="651" alt="Capture d’écran 2024-05-16 à 23 40 32" src="https://github.com/ultratwo/sybilled20/assets/160050412/8f419f55-e137-42ca-9daf-d368a96705ad">
https://etherscan.io/tx/0x6caab745b707eb195cdfe38247afa3f9e9662aa4312bad8d8955f8b7c910ac1e

<img width="622" alt="Capture d’écran 2024-05-16 à 23 40 39" src="https://github.com/ultratwo/sybilled20/assets/160050412/173188dc-38f8-412d-b9f3-68a6e249ffd6">
https://etherscan.io/tx/0x558ce24f0670cce3d4baf4662927dd504411cace0b81386142aba518f4828bf1

<img width="647" alt="Capture d’écran 2024-05-16 à 23 40 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/56d39644-f613-4850-b6d5-bda802a7a10a">
https://etherscan.io/tx/0xda31af23f94d07f1c254402c4e972f5ebc990db66f5c20cd3c986158f609c314
<img width="645" alt="Capture d’écran 2024-05-16 à 23 40 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/541d4399-fbf9-4dcd-88af-4a6408c9ff39">
https://etherscan.io/tx/0x129617a27d3f566960ebb2e153ae181186b5e2f4cfb85954adc058284f06fbdc


<img width="670" alt="Capture d’écran 2024-05-16 à 23 41 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/eff0011a-c5f7-4078-bc8a-497b8885bd00">
https://etherscan.io/tx/0xb664acb560a7a546cde2f28f940a01d96e3499daba85192bc07d8af9d65e6573

<img width="672" alt="Capture d’écran 2024-05-16 à 23 41 07" src="https://github.com/ultratwo/sybilled20/assets/160050412/102a428e-0313-4e1c-84c2-725ed9bece69">
https://etherscan.io/tx/0xbdcf11ddc3fe45aa5f0145e077dd68d3273c372d58cf421a97c52a7678eb13c5

  <img width="665" alt="Capture d’écran 2024-05-16 à 23 41 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/cfb015e6-f0cc-4ec5-ab57-d6dfa4b99d0d">
  https://etherscan.io/tx/0x416ae039a400a4f9e2be2d229e75e7304d81b18234d3c38c279246cfa53c48a8
<img width="691" alt="Capture d’écran 2024-05-16 à 23 41 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/89963f44-64cc-4fa2-b1cf-fdc5ff3f478f">
https://etherscan.io/tx/0x5a6192dfa0b1a916158ff7516c3158137e46cb8e2dca1c23724bdce0d219d0fa
</details>



Another example is the addresses used Stargate on Polygon with similar amounts of stablecoin (25$ approx) the same day (48 hours timespan)




<details>


<img width="676" alt="Capture d’écran 2024-05-16 à 23 47 41" src="https://github.com/ultratwo/sybilled20/assets/160050412/4552bdb2-6f76-4be7-ab29-25eae972b8dc">
https://polygonscan.com/tx/0x205fff499e64fd70e4df3c28b477c48ee7b4aa7fca9c554aa69dea18788d7f7e

<img width="652" alt="Capture d’écran 2024-05-16 à 23 47 54" src="https://github.com/ultratwo/sybilled20/assets/160050412/f378df04-5569-4128-9eea-45c3947dec92">
https://polygonscan.com/tx/0x0d4f870b2d6fc8c3a5ee805c64a3ff4edcf8c4da34f5db1c80bdd7b6e26feb2c


<img width="686" alt="Capture d’écran 2024-05-16 à 23 48 03" src="https://github.com/ultratwo/sybilled20/assets/160050412/6cd29296-b6c1-4c3b-9bac-b369d4f369c6">
https://polygonscan.com/tx/0xd71370c69ec8b91a4b04ce9706173671a29a686b559b11e054b45279bd0a7b3c

<img width="665" alt="Capture d’écran 2024-05-16 à 23 48 10" src="https://github.com/ultratwo/sybilled20/assets/160050412/28a21080-8ac5-4f63-93ec-1d5e6de39471">
https://polygonscan.com/tx/0x7f05e120fdec4e3709bc30eb08ab56e22d18b2c0a40c1f63ac976282ce7cf3a9


<img width="661" alt="Capture d’écran 2024-05-16 à 23 48 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/de84b95f-6570-45aa-bd66-736cfc190903">
https://polygonscan.com/tx/0x75a93d6f398f0a409bce112a337bf35b2eecd86dc3837ea96d2cd2ac5b936002



<img width="656" alt="Capture d’écran 2024-05-16 à 23 48 23" src="https://github.com/ultratwo/sybilled20/assets/160050412/c774e7b3-3a0c-4ae1-9796-ace1f366b2f1">
https://polygonscan.com/tx/0x7429237788d4dab7d3f512f98d3bf57eefb2e8ce44cf53a7c78762488af3a904


<img width="663" alt="Capture d’écran 2024-05-16 à 23 48 31" src="https://github.com/ultratwo/sybilled20/assets/160050412/ae95d7b4-4d46-447b-9aa8-f0cf227c3706">
https://polygonscan.com/tx/0x04c5066a4522a593570c0a913b2747b4412e646bde4a2cbf10ec8bdbdfc91569

  <img width="652" alt="Capture d’écran 2024-05-16 à 23 48 37" src="https://github.com/ultratwo/sybilled20/assets/160050412/a32e4c92-f89b-41a4-a539-28ee44e340bc">
https://polygonscan.com/tx/0x26a02d855a3b199e3cffd1c535144595b9e6e5c155e456a7bf2c91d82b04815f
<img width="669" alt="Capture d’écran 2024-05-16 à 23 48 45" src="https://github.com/ultratwo/sybilled20/assets/160050412/ea385cf3-9de1-4d81-800e-aa5313e7b61d">

https://polygonscan.com/tx/0xac27cf0f610b7313eb68370d866ef541f7d7447c7780ac452603254e20de1dac

</details>



Cluster + same CEX deposit address + same on-chain activity. This is a clear sybil cluster.





## CLUSTER 18






The first 11 addresses of the cluster share the same Binance deposit address 0x2e83C858470b9C871Fe046f8d14734796CD2a604. The rest are linked to numerous addresses of the cluster, multiple times.

11 addresses were present in Nansen's report and discarded.


```
0x7d0b61474564fdedee5b711b5bc370d636ab6794
0xbc23b26568ce8ed7c3a0f576512c4a5bd7442ede
0x85e830e99e718ab7a5c6f129ee5e3449a81f9bfd
0x3b1939dae2c4c97a7b74bedc83c1a0c5673b2b1c
0x2a68272f9ed46c0141494b4c7949c3fb40801683
0xfaaed57b13bfc1e89f636b05594bfe7113706509
0xf11dd9a09036d23aa59c8684f021974f2e42a6fd
0xe5b75b26e453f7947e606230ebc576abe862cc29
0x0abf6c46bf2eed15da3509adb6eba1a2285d8563
0xd838efba49e0816fd8c2d3b52c0b4632f030fd8a
0x4e79f7c7deed79c53e73c6333bce526d33c07c8e
0x294505b89f9621fb06e93a47af70847b2484020b
0xbe71a7993d0ba3c7f3ece9dc8c108ea9f0699297
0x8074b1285c0fba1f4f9d0ef586c274bd1e2fa509
0xfe7408caeff03e70d6be1a060298f6d425e81ee5
0x1871f42b4bafeaf5fb95cdc57d32820ff687fe74
0xf38ffae62d44bb3742ffa77bc2988df44da449bb
0x3909e2591c958ef17e61092b891e63f9ba34519f
0x5ab9125a5a07797432b022e6f9b573f23c34a012
0x8d37ffa50ac1efcc0c1c0c52e6741433f3793565
0x9e8c3a8c7f7297a9a5cd9868f00c311157d88dc9
0xa72ac575ce5d86876b43b2ac073ecba2b997db2f
0xd8e19e1d065f6fceda9e8dce74489e65abc53518
0x16502dd135c35375630421bdd58155cfcd0927e1
0x611746441d926c014a75b145788f11f0078f1bad
0x514efc11603d5bc5e8facd58c46f5af2b16dc406
0xb0634731f0adba7d694a192d1713d5c66bbad832
0xce089c06f40737683143ea7eaed4f773f1492c44
0xde280a28b3a55b976d11bfa5cd6982efa5169a59
0x49648311eb4136b8a1574b883bcd38f9eed0261f
0x102ad0751533b924f2b5fb68c299fe44d2112be8
0x6e835cd1ade6d2e5edaeff85c9b778c148451e68
0x2af8f640c839544044334daf6d9d124efc52260b
0x6f8b5a36e967362818850140f7296651f3528f35
0x24719685efa96fcd19d31703f5291c3f5a4eefc7
0xc6f4eefab5d79a292e22a43d83886f6432a52b10
0xafb84fd963f5f64c58e1a2e63d925634ebcebde5
0x5462ce18647ef432b55726d4f60292049b1146e5
0x42dfba02e0ab9ef00a52061c8b8350ba0f685ba8
0x1a93fce8758ac97bf3fa780f85fe58873985bf03
0x2bdf809fde9655f696bc47551653a2613e2ab4a1
0xe966a66f66e9de4477fb51b7a8112ace880febb3
0x8305b3ac78c60a84d150a9ee6b7d72b0c08a2475
0x20a3eb17ce456a5c4a38c437665523d94634ec8d
0x126cb9ce08aaa9d9920b542d9021a789be986008
0x8ae5f55ab6be05c7b98bee1f9cb597abe929b7dd
0x2ab4a96ca02862df402fdd939d48d4de5c626191
0x3d096a48dd10802b4ef89c5b7e9d590e6223799e
0x99437ad0c95435e860dfb2e6995626b3d8809a2e
0xcf92e4330c881642f41a0572189101fbebbf1a64
0x022f4b164cbe1b5c65ad3518f7a1b1097ae2015a
0x071c0f18824e57690aafbc9ad7627089b626f6c1
0x0c6037f43ed9b6ba6499ebcc710aa8b18a07caf1
0x0f97b76613fbc23e66f2c51667ab802639a91066
0x129652436238f664e0df2f806533cc9792d4c5b5
0x15578a892ebd3e98ff7ece5b718129a4dc1b9f32
0x1941d8f1d75d408f41fd37ed30e2ead142a6702f
0x19b87e31be53dba547bb2c09bfac6451d3c23211
0x1a056a2cf4cfdc7ab6f27eed8baea43886f6ab40
0x1a642aadae94b892f34a51cdf0af04d5d761b1f4
0x3071aea7ae75d0ed5830a84f240334b92a91702e
0x36dc8895f26ea36d7afc5a8c0c2370c1cf415015
0x387028e8d4b94f72bf4f3bbc43380a9a10f69da7
0x3cc026c75caf73347371ec4d78dd82424ef022e2
0x42f6725e27f4500779815217f811de304f17d353
0x54048fcb8afba9ac2c2d68b4a5c504bc4ce39c5b
0x5c866f4ba4146e12824f3b48e7d61d93e1d5197b
0x6413a4f28fb8a58fd76c28fb4ae958722cc578b8
0x65b06931ba923d661769198c38247f1949c9f7ae
0x7e35e86772797e9e0fa55681e483c56b8885b545
0x874f51a45614d249088de4c853dc1a5640e4f004
0x8c316b6b9aaf9fa99567c8ac6593433fc53441e7
0x8cf531818fa432519a55fad0cafa44a5f27173d8
0x91d415c63630f45188e754c6aa722ac0811eecc1
0x91f5f9e08ccc611ef9fa5f18ec717f58d4e8aac8
0x97a30c15f192dd4a59bd40ff930159b8b58db2c2
0xa22ecaa973364d4e88d2cc88811eada868660041
0xa64fcc82431c7388e8a15a7b5c0bdbf492bde699
0xb7a8969219f2f8108fb8dac4b30cc944c1cd833b
0xb876444a716388c3910cca7f3ca64ab25d920c9c
0xc65af0594229acb4877a28ea8b987d80e79d65a4
0xcee1d37d413c49688bed52db589653523e87bc2b
0xefc8b6e5bdda8fc9b46ae96bf8cf3a280da96f94
0xf4e02a4b969302d4f4d34c2cabd984647177bc94
0xf99c577c80458e9d2f5475742dbbfa5739cd407f
0xfb14a723449440b3e93630edd56d14945b4a04e2
0xfd9e3d221a5d36f15b151a85543edfb7053df50d
```

<img width="627" alt="Capture d’écran 2024-05-13 à 16 29 07" src="https://github.com/ultratwo/sybiled/assets/160050412/dabf7271-2957-495e-afaf-9010299f39f6">


The addresses of the cluster have the same on-chain activity. Their first L0 interaction was either 734 days ago, or 366 days ago. This is a sybil cluster those all addresses started sybilling at the same time (the sybiller added two dozens addresses to sybil later)
<img width="1120" alt="Capture d’écran 2024-05-13 à 16 57 56" src="https://github.com/ultratwo/sybiled/assets/160050412/e7fdbfbb-ca5d-4cfe-b9c0-c8bebcf76ae5">
<img width="1112" alt="Capture d’écran 2024-05-13 à 16 58 11" src="https://github.com/ultratwo/sybiled/assets/160050412/4e564f7f-2df6-4388-889a-0de6ce75ca0a">
<img width="1113" alt="Capture d’écran 2024-05-13 à 16 58 24" src="https://github.com/ultratwo/sybiled/assets/160050412/291c0fb4-4799-4529-9812-b43bb6afa689">
<img width="1105" alt="Capture d’écran 2024-05-13 à 16 58 38" src="https://github.com/ultratwo/sybiled/assets/160050412/9a457179-ce6b-4097-b3ef-b8703d213bc3">

The addresses of the cluster follow the same pattern for their Layer zero interaction, probably because of the a script. For example, their latest L0 interaction always is the same: the same DAPPS, Stargate, Maverick, Orderly and Holograph in the same timespans.

<details>
<img width="895" alt="Capture d’écran 2024-05-13 à 17 07 40" src="https://github.com/ultratwo/sybiled/assets/160050412/d1342ae5-1cb8-4056-9942-9349e6befe03">
<img width="897" alt="Capture d’écran 2024-05-13 à 17 08 16" src="https://github.com/ultratwo/sybiled/assets/160050412/f972beeb-8468-4ada-96b5-9668d7b5a493">
<img width="889" alt="Capture d’écran 2024-05-13 à 17 08 28" src="https://github.com/ultratwo/sybiled/assets/160050412/5965eeaa-f4e3-4578-8ff6-4716cde25a78">
<img width="901" alt="Capture d’écran 2024-05-13 à 17 08 40" src="https://github.com/ultratwo/sybiled/assets/160050412/230abcce-6fc8-4c16-a61a-ad78ca3c43e4">
<img width="905" alt="Capture d’écran 2024-05-13 à 17 09 07" src="https://github.com/ultratwo/sybiled/assets/160050412/a09d90d4-0ed0-400f-b191-29ff3c628a45">

<img width="885" alt="Capture d’écran 2024-05-13 à 17 07 48" src="https://github.com/ultratwo/sybiled/assets/160050412/4c32da03-9afd-4ce2-9152-228356eb538a">
<img width="887" alt="Capture d’écran 2024-05-13 à 17 07 56" src="https://github.com/ultratwo/sybiled/assets/160050412/4c6d615e-fc21-412f-9fd8-c97ac027d58a">

etc.

</details>

Their interaction outisde of L0 also is the same. All addresses of the cluster follow each other on Debank in an effort to farm the Debank airdrop. They all have 100 followers & 100 followings approximately, and TVF of around 90k$

<details>
<img width="521" alt="Capture d’écran 2024-05-13 à 17 10 20" src="https://github.com/ultratwo/sybiled/assets/160050412/d949490d-49a0-4fc9-a5b3-137160b63006">
<img width="355" alt="Capture d’écran 2024-05-13 à 17 10 27" src="https://github.com/ultratwo/sybiled/assets/160050412/0c3ffa23-cd6b-4a0c-8291-0aea14012c18">
<img width="354" alt="Capture d’écran 2024-05-13 à 17 10 44" src="https://github.com/ultratwo/sybiled/assets/160050412/ad45a554-eeb4-4dd6-908b-05e7ee793e79">
<img width="356" alt="Capture d’écran 2024-05-13 à 17 10 51" src="https://github.com/ultratwo/sybiled/assets/160050412/a2cc1a26-b4a1-4c96-a4b1-711ae1ae638d">
<img width="354" alt="Capture d’écran 2024-05-13 à 17 10 38" src="https://github.com/ultratwo/sybiled/assets/160050412/34c8f3a3-08e6-4c88-b8b6-8088a0567fbd">
<img width="354" alt="Capture d’écran 2024-05-13 à 17 11 03" src="https://github.com/ultratwo/sybiled/assets/160050412/155b0261-ffd2-4a75-95c2-233402ab7caf">

List of followers of one address of the cluster : https://debank.com/profile/0xfe7408caeff03e70d6be1a060298f6d425e81ee5/follower

<img width="111" alt="Capture d’écran 2024-05-13 à 17 11 47" src="https://github.com/ultratwo/sybiled/assets/160050412/2e09d506-652a-423b-aa06-b2b865cf2b07">

98 out of the 100 followers are part of the cluster.
</details>

They provide liquidity/stake to the same protocols in an effort to farm multiple airdrops accross 98 wallets,ZeroLend on Linea, Sturdy V2 on Mode, Staragete on OP etc... The addresses also have a lot of dusts (<0.01$) worth in the same protocols, this is the trace that they all used the same protocols. Not only they use the same protocols, but they also do it at the same time. For example, the addresses of the cluster all conducted the same transaction the same day: they all placed a 0.01 ETH bid on Clusters the 9th Feb.

<details>
  <img width="485" alt="Capture d’écran 2024-05-13 à 17 14 45" src="https://github.com/ultratwo/sybiled/assets/160050412/b094a1c9-e450-4a20-aea7-ab98439c79fb"> https://etherscan.io/tx/0xd2a319f1c0dde2144e461ace6af1de0889b3880f525b4cf9fee0c1b5ca905494
  <img width="479" alt="Capture d’écran 2024-05-13 à 17 15 16" src="https://github.com/ultratwo/sybiled/assets/160050412/f493033c-7344-42cf-8514-3c903a475f06"> https://etherscan.io/tx/0xb950f66d80928643430444ba69d892d508fb93351173822a908e8beca1cebb0d
<img width="481" alt="Capture d’écran 2024-05-13 à 17 15 41" src="https://github.com/ultratwo/sybiled/assets/160050412/3ed6bb50-d84c-41be-bab8-b2aa35a3b94d"> https://etherscan.io/tx/0x4c6a18d6476ff672f6debaaa77bd69860e379f7cc42213c7ac529fd28dba7017
<img width="797" alt="Capture d’écran 2024-05-13 à 17 16 12" src="https://github.com/ultratwo/sybiled/assets/160050412/2462e205-3a20-4614-bead-a5500d1c4a8d"> https://etherscan.io/tx/0x77a6098e941597b2e8e83a4f772c24d932c9c90175bbb9bec4612d628986d595

<img width="502" alt="Capture d’écran 2024-05-13 à 17 16 30" src="https://github.com/ultratwo/sybiled/assets/160050412/66a804f2-95dd-4dcb-b1d8-0c0e63cab9d9"> https://etherscan.io/tx/0x1e9e5bdf622864cc9eabb9a39cb2297b0922642b93d5de96e7e0e9d4e6bce670

<img width="480" alt="Capture d’écran 2024-05-13 à 17 16 48" src="https://github.com/ultratwo/sybiled/assets/160050412/2c83a596-3fd5-4bff-9f82-df31cf5c1f90"> https://etherscan.io/tx/0x86ca322b1e072df8d0af5acd2bbd7d4ee2b9cca96c72a895d372f1f339bcb644
<img width="625" alt="Capture d’écran 2024-05-13 à 17 17 10" src="https://github.com/ultratwo/sybiled/assets/160050412/4b29c4f3-662a-48f5-b2f6-c408b7424f81"> https://etherscan.io/tx/0xc8b509274e9f8b512620d5f50c8fddab0ef9ca42eef569fe558fe8cf54378a64

<img width="719" alt="Capture d’écran 2024-05-13 à 17 17 30" src="https://github.com/ultratwo/sybiled/assets/160050412/fb810375-960a-4938-860b-fc9faea8da2a"> https://etherscan.io/tx/0xc8a48d89e486a625ea6a71bcb47fbb213dd446ae38a86b4a65b7d1bd901c40af

<img width="620" alt="Capture d’écran 2024-05-13 à 17 17 50" src="https://github.com/ultratwo/sybiled/assets/160050412/b1db7720-83eb-4d7f-9a69-24a3bd1ae446"> https://etherscan.io/tx/0xd8699bffa21e2b31e16bb7bc4bce6231ef21ebedcce8957d394471dbac7b99de

etc...


</details>

Another example, all the addresses of the cluster claimed their Omni airdrop and deposited the same amount of ETH intoRedstone Bridge in the same timespans.
<details>
<img width="767" alt="Capture d’écran 2024-05-13 à 17 19 41" src="https://github.com/ultratwo/sybiled/assets/160050412/a6deb840-ba69-4dc6-8227-6b6b59afe3a6">
<img width="753" alt="Capture d’écran 2024-05-13 à 17 19 51" src="https://github.com/ultratwo/sybiled/assets/160050412/108c27ed-9bdf-4f0f-be2e-10f9dc7d3245">
<img width="728" alt="Capture d’écran 2024-05-13 à 17 19 57" src="https://github.com/ultratwo/sybiled/assets/160050412/112db134-bd30-458b-9620-f2b3d613e955">
<img width="752" alt="Capture d’écran 2024-05-13 à 17 20 09" src="https://github.com/ultratwo/sybiled/assets/160050412/c3cbf659-7090-4197-9aa7-c2d017da921d">
<img width="772" alt="Capture d’écran 2024-05-13 à 17 20 15" src="https://github.com/ultratwo/sybiled/assets/160050412/08f1ac5f-5575-40ae-ae54-55d00aeca160">
<img width="752" alt="Capture d’écran 2024-05-13 à 17 20 22" src="https://github.com/ultratwo/sybiled/assets/160050412/cb4943be-ca05-4221-ba97-58c10df4ee7e">






</details>

Considering the cluster, the usage of the same CEX deposit address and the exact same on-chain behavior, there is no doubt this is an industrial scale sybil cluster managed with a script. This cluster already claimed numerous airdrops without being detected.







## CLUSTER 19




The first 22 addresses of the cluster share the same OKX deposit address 0x2d045EdD5F7a744f3b4090bb61c8623A0996C5A7. The rest are linked to numerous addresses of the cluster, multiple times.


```
0x046f601cbcbfa162228897ac75c9b61daf5cee5f
0x706cf81141ca1f173369001037d3958ecf6dc8fd
0x05e818959c2aa4cd05edae9a099c38e7bdc377c6
0x256e96a8c01d3cc5b185254dbe553fe3c258e8b4
0x167dd1517b4ca5520aee35ca680b7080bbc1f75e
0x3084409978c7dec5f968edbbafe368fe814b299b
0x6c8af157dfc3f9b25e62ac8b9ddb01365d909be0
0xad4d386d52b8824e45373aebfa9f62f64ec0a46b
0xef831b62943a04098a10c5161674e3e13d5d3377
0x982ec8f00e2b6e3355ed63de1c28fc982078d39d
0xce0d5a671b645c4f3df390971186477dfa5e7c11
0xc06e9f79235355d92a405965e6b9eb15142d35e3
0x4645a30a4051e4aa9ba57c2158b97d2ef4995fe7
0xd5d0a20c8cb66e3fa10e0a4558eaf72d841209c3
0xe162377ab8327c5bbd20bdecc26dfe8b5e47bee4
0x156e1bc3e63f790329e574fd837addf510d5af19
0xca1f877a43a3d2dce757b8d9be238828b1125a4b
0xd5fc0e024b553ff5b02648b40d4a3722cb21eeae
0xc5276d9a1e7ba137bbdb0107ec634ee61f01c31d
0x229055716201137496061c8ec9d6f734c510437b
0xfcc5301f91accf8c2d8e826c18dea7107e7303f3
0x53e755c64342457c36fa97a4fff9f040f74bfb09
0x88cf03e4a797f16a8be621eb8dc6f710e7ed6104
0x209168d87544fa3faa3fb27736613d517b04010e
0x34989d4f974617f9988164e1af1b512ffaf37fd8
0x51938a3d47070cc226143d8aab1aa048f757c292
0x5b5e41f0dd67e52be4b2eda309cba456542a2d69
0xd24604509d93d62c471a7f681e0488962a626236
0x35179fb95d2ac3d8fdf30ebb9af43f25a8778d41
0x43c74d5cd7c07d06ad773e2f93605a9d48695fc5
0xf5799cadf29008fdbebfdfe789f9b84f4cc23246
```

<img width="741" alt="Capture d’écran 2024-05-13 à 12 30 41" src="https://github.com/ultratwo/sybiled/assets/160050412/757afda5-0beb-4e7b-97f1-1527e9adf6b3">


The addresses of the cluster share the same on-chain activity. For example, they have the same L0 interaction pattern. They use the same L0 DAPPS in the same order in the same timespans: Stargate, Aptos Bridge, Maverick, Testnet Bridge and Holograph. 
<details>
<img width="914" alt="Capture d’écran 2024-05-13 à 12 34 17" src="https://github.com/ultratwo/sybiled/assets/160050412/4e053ad1-e7b9-4351-9500-d6ca0bfb25d1">

<img width="892" alt="Capture d’écran 2024-05-13 à 12 35 45" src="https://github.com/ultratwo/sybiled/assets/160050412/1a247fbc-22be-422e-b679-8ffbf3410da5">
<img width="901" alt="Capture d’écran 2024-05-13 à 12 35 53" src="https://github.com/ultratwo/sybiled/assets/160050412/7e9f2a9a-dd6c-435f-acd4-79d23c748a8f">
<img width="915" alt="Capture d’écran 2024-05-13 à 12 36 03" src="https://github.com/ultratwo/sybiled/assets/160050412/f3112d74-84f2-4afb-8c3e-67f17f3a0f3d">
<img width="906" alt="Capture d’écran 2024-05-13 à 12 36 15" src="https://github.com/ultratwo/sybiled/assets/160050412/2b19016d-2f04-4e3c-8dfc-50fe29a60eab">
<img width="907" alt="Capture d’écran 2024-05-13 à 12 36 22" src="https://github.com/ultratwo/sybiled/assets/160050412/c206990b-a213-4761-99df-ceabef637ebb">
etc.
</details>

Considering the cluster, the usage of the same CEX deposit address and the same L0 interaction pattern, there's no doubt this cluster is of sybil nature.









## CLUSTER 20


The first 10 addresses of the cluster share the same OKX deposit address 0xd0BF249F4dDd7F4dc1A8b788D9880a7371dF13F6. The rest are linked to numerous addresses of the cluster, multiple times.



```
0x25ed13960fa2287026d4cae16954c9d21cb1b2ff
0xa66e9723ac3ad3b0c76014ace3ca10304e8cf68d
0x5300628cf0bc2ea1ab9b8773d0984de9927989ec
0xda4b02f4b7612ba6b8c6fbc8227d0ec5544c32db
0xc2184dbc04bbef88353b3a9527cfad0f0f1d4bf8
0x7e7a932b832afdac19895aaa0d7607fe56c46838
0x5b0a3e243ed4153eff4faab20a342fcc69ef13db
0x97edadcb850fe4783fae7f41c8d8953461b6e363
0xc8502840918a2dbc6554678a27dee96261acd090
0x200210d9ee8356055e887e7ee96d4333d8f2ed38
0xe292be8e3f302749b574c217879d6fa829925797
0xf9c57a27a8aef74548213b66b76c522017c4b863
0x0071ae9bc6ca4779357974b1f977d10b73e83e14
0x6906d762732497ed18fcd9bf1af63eb8afb9116a
0x7007fe3a274a0e9ddad20ecf9b603a99a14a3b12
0x1e7b716765f017bcca696edff9969abc514b6ffe
0x6a6425e29334ff4b70e54d4afc5f795354c2b514
0x1489cd7378cb777e0a525813561c6fa72d4e64c5
0xa799e684466e47bdb3ee0efd9548bc7edc28e05f
0x57ef43c7f7e9bd53b024f8162917b66ee129a4c0
0x29df692fb07efe1ee5a58b038f91feaf793e104b
0xc960ebdc4155d67a8c465ce0349d05d42e038668
0x3225a91281a6da274721641c4018b3fa52f606cd
0x0cabb748ebebe0662f9fc7f2f9ad1b9138e5aef0
0x3d5ca0a0277b1f8dacc67c80a538ad2f9546c602
0xcbecd3b0dbd86d8c6f533cca128da1af9ec91969
```






<img width="569" alt="Capture d’écran 2024-05-17 à 02 34 43" src="https://github.com/ultratwo/sybilled20/assets/160050412/f4822b12-d067-4918-8ace-44f3d20743e4">




The addresses have the same on-chain activity. They have similar LZ Age (date of first L0 interaction), amount bridged, contract count, interacted source chains, Unique Active Days etc...



<img width="1107" alt="Capture d’écran 2024-05-17 à 02 35 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/399a4ddb-cc7a-44c8-acb1-03416abb6b28">



Their L0 activity follow the same pattern, probably the result of a script. For example here are their latest L0 interaction, same dapps, same timespans, same order, same source blockchain.

<details>


<img width="897" alt="Capture d’écran 2024-05-17 à 02 38 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/97da22cc-b307-47d0-954d-242b112bb7ad">


<img width="898" alt="Capture d’écran 2024-05-17 à 02 38 16" src="https://github.com/ultratwo/sybilled20/assets/160050412/e53ec8a2-fa76-4e6d-b6f9-d97280f9cd1f">

<img width="879" alt="Capture d’écran 2024-05-17 à 02 39 27" src="https://github.com/ultratwo/sybilled20/assets/160050412/f0900405-d81c-4cea-aa98-7ddca3279014">


<img width="911" alt="Capture d’écran 2024-05-17 à 02 38 22" src="https://github.com/ultratwo/sybilled20/assets/160050412/48dbbdbf-fa62-4929-9e4d-614a2aa6723e">

<img width="888" alt="Capture d’écran 2024-05-17 à 02 39 19" src="https://github.com/ultratwo/sybilled20/assets/160050412/2324de9a-d5dd-46ae-b64e-15c3e82000ce">


<img width="909" alt="Capture d’écran 2024-05-17 à 02 38 32" src="https://github.com/ultratwo/sybilled20/assets/160050412/6c39ad8d-ea0a-4ace-8ba6-2250607271ba">

<img width="897" alt="Capture d’écran 2024-05-17 à 02 39 09" src="https://github.com/ultratwo/sybilled20/assets/160050412/b09d59bd-8508-47b4-9735-861586fea8f0">


<img width="907" alt="Capture d’écran 2024-05-17 à 02 38 48" src="https://github.com/ultratwo/sybilled20/assets/160050412/99f6eb65-386f-4717-bd84-5f56556f70ef">


<img width="903" alt="Capture d’écran 2024-05-17 à 02 39 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/5f1f2e30-5c3a-4f53-918f-07027971f012">

<img width="896" alt="Capture d’écran 2024-05-17 à 02 38 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/1a4cc880-d30d-4e77-9a4e-544f6329014c">







  
</details>


Cluster + same cex deposit address + same pattern farming airdrops.



## CLUSTER 21



The first 10 addresses of the cluster share the same Kucoin deposit address 0x4EEd863789F58470f6b0e7b5cE3458793e5d2636. The rest are linked to numerous addresses of the cluster, multiple times.


12 addresses from that cluster were present in Nansen report and discarded. Same thing than last cluster, some screenshots and links may contain those discarded addresses, but the argumentation stays strong, stronger even.

```
0x602c47c1f13d91c05dfed0f23587020415f0e524
0x2a17ccee60e0b5642b2e7ff3a5246d7e028e2e9c
0xbd05a53ce69a5eb3c3919d90a4817a2ba0a75f10
0xbed6d14ecced7994bba2c7f9ea210b605380b73f
0xc19ba152d9fa90854ffc51ecb41ec3bbfeb97705
0x7360e2f6eed8244f35b1070f6fe3d10dd20a22f3
0x3a4c18f4cce58895eefe3985d91bff17c1420226
0xcd1b8644c58d5691e2de12ecc1a740e7ae7a4251
0x83d0d03f76aa04c8e0eb58d5ad51ebe739be18db
0x3a6e34f3e1ee44f1e4605388815b0b7df783838a
0x20ac42a33f2e942b3948eaab51e0acde7370eeec
0x7b665f4a8a504c09a7f6931628f8b9c054638bae
0xdb9bfbd9ff49877d691bfe0bc22673b2c1a9f161
0xde924aa663bfaae0b63191e9843df255889c907f
0xf4238bf7d4cba389c7eedbb1eea6bc0fc93c1a47
0x1c6ba0fd9fd74fd7dfd04e1d7eb763e4f2faf62a
0x3fc872c93193f63505f7d710591ff8b75f1b3f70
0xe9c8e840937632ac7eeb01ae3f04695deb5b9781
```

<img width="546" alt="Capture d’écran 2024-05-17 à 16 12 13" src="https://github.com/ultratwo/sybilled20/assets/160050412/1ab854be-9f52-46e6-a3c8-c2ced8790698">

The addresses have similar on-chain activity. For example, they all bridged similar amounts of ETH using the Zksync era native bridge the same day (48 hours timespan) in order to farm the ZkSync airdrop.


<details>



<img width="640" alt="Capture d’écran 2024-05-17 à 15 49 25" src="https://github.com/ultratwo/sybilled20/assets/160050412/4f343557-0667-44c2-893e-daf3e1b345c8">
https://etherscan.io/tx/0x01e051fab77a9a02cf7b1330b06f0cb93826031ffbd284d46d5911609db1ea88


<img width="668" alt="Capture d’écran 2024-05-17 à 15 49 34" src="https://github.com/ultratwo/sybilled20/assets/160050412/2ced202c-348b-4796-a505-6ba4a35c2f3a">
https://etherscan.io/tx/0x558ce24f0670cce3d4baf4662927dd504411cace0b81386142aba518f4828bf1

<img width="663" alt="Capture d’écran 2024-05-17 à 15 49 41" src="https://github.com/ultratwo/sybilled20/assets/160050412/d640b84a-9a09-43f5-a4b9-d669f0d082be">
https://etherscan.io/tx/0xdbb7fddc65b0517b753a7fe306db2d888fa4b4bc4b700c85c62ca977a23445c1

<img width="643" alt="Capture d’écran 2024-05-17 à 15 49 52" src="https://github.com/ultratwo/sybilled20/assets/160050412/9419938a-8177-4b1e-9b2e-9e172c7a139c">
https://etherscan.io/tx/0xc68f0188ed1ecc9e9268feb9d97905463f55604559729b0725b27b212ce8d276

<img width="656" alt="Capture d’écran 2024-05-17 à 15 49 59" src="https://github.com/ultratwo/sybilled20/assets/160050412/6a2456ad-9fdf-40c1-81e4-e3290ebc8694">
https://etherscan.io/tx/0xb664acb560a7a546cde2f28f940a01d96e3499daba85192bc07d8af9d65e6573

<img width="648" alt="Capture d’écran 2024-05-17 à 15 50 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/39fa34e9-6a9a-4ab4-a598-c322f6af8b0e">
https://etherscan.io/tx/0x129617a27d3f566960ebb2e153ae181186b5e2f4cfb85954adc058284f06fbdc

<img width="647" alt="Capture d’écran 2024-05-17 à 15 50 17" src="https://github.com/ultratwo/sybilled20/assets/160050412/acf23f15-e9b0-4510-a07d-fc7b46bbd40b">
https://etherscan.io/tx/0xda31af23f94d07f1c254402c4e972f5ebc990db66f5c20cd3c986158f609c314
<img width="667" alt="Capture d’écran 2024-05-17 à 15 50 22" src="https://github.com/ultratwo/sybilled20/assets/160050412/784b807c-b69c-42f4-a9cf-0c3404bfb0fc">
https://etherscan.io/tx/0x0bcffd6e70009bc2274d73474be2fdb9e1eb43ed99d4f9385fdc44923a438ae8
<img width="640" alt="Capture d’écran 2024-05-17 à 15 50 30" src="https://github.com/ultratwo/sybilled20/assets/160050412/ec533d1c-17bb-4cdb-b666-f0075333750b">
https://etherscan.io/tx/0x5a6192dfa0b1a916158ff7516c3158137e46cb8e2dca1c23724bdce0d219d0fa

<img width="657" alt="Capture d’écran 2024-05-17 à 15 50 37" src="https://github.com/ultratwo/sybilled20/assets/160050412/e9afbf17-111a-4983-a27e-f7a011527043">
https://etherscan.io/tx/0x034c7c5063400cbac5ecec8bf4e2315e36c8fb3c46c8ad37563c697f646de260
<img width="632" alt="Capture d’écran 2024-05-17 à 15 50 44" src="https://github.com/ultratwo/sybilled20/assets/160050412/8c2056b4-aed4-4731-a5d1-0c7922c9405c">
https://etherscan.io/tx/0x96cbfda65657e03a3055367f4407375a7e745d6f0205d0d7c99dbc4f1a23b884
<img width="652" alt="Capture d’écran 2024-05-17 à 15 50 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/8308a11c-77bf-4064-8389-21669318f476">
https://etherscan.io/tx/0x8b979240bc93e700a927cffb7fd2f07b615addf6b80c4136b6fe060d0e96d428

etc...

</details>

Cluster + same cex deposit address + execute transactions at the same time with same amounts to farm airdrops.





## CLUSTER 22



The first 14 addresses of the cluster share the same Binance deposit address 0x7d7Bb79008312b1cb67d75C6f6567023b1a37800. The rest are linked to numerous addresses of the cluster, multiple times.



```
0x5999a1679dc298b31d490c44759cb1e496483622
0x031033758c8efbb011daab00125ad0e87649b2e8
0xa1599ff567ab55998487cfd380a31a82e1fe8bc6
0xad6f3453775d9fff7c49508479533deb6e83e369
0x764d46d2256bc755d87880ad2114911a5736a0b9
0xf3f5a79141994fc4129d25ca3d9ef31f9b0381d1
0xfbed510ad37362283fb1f93e87b3501815833872
0xa56dd1e551d7e191870c1228b945116d3785c75c
0xec6fcd4e8cbe72e9a91029b980eab4127617bed6
0x51eebc665f2f61864674c2b446e6d0891bd26115
0x31cacfb035444c73238703b1e856e3a250fd4ec8
0xa5976e7979fc67591b8205cfd28e7e753190855f
0x50e2e0b012fdd2acc5088eafe948bd9547e38f8f
0x47813916b6ebcef0b4147ca77852110fe157754d
0x6bdd966ddb230e835778339265823cfbd270abac
0x1467ba04f9b26dde77959e99bebfe198f174da9c
0x4e51ad017b453c28bf4b446d99d287960f61fc9d
0xbb85d122f28ff2e700f7768d55c275a08617578b
0xb7bb5a9e342ac044bbc3ef662b9211673f1b4aa5
0xcd28e2b471f1847bbb40a2b99868b175f3f4f137
```



<img width="401" alt="Capture d’écran 2024-05-17 à 17 11 10" src="https://github.com/ultratwo/sybilled20/assets/160050412/bc1c84fa-12f8-4b05-9d52-7e5cf64ec0f5">




The addresses have similar on-chain activity. For L0 interaction follow a same global pattern. For example, here is their latest L0 interaction, similar dapps in a similar order and similar timespans.

<details>






<img width="897" alt="Capture d’écran 2024-05-17 à 17 14 26" src="https://github.com/ultratwo/sybilled20/assets/160050412/cda99d33-3006-4756-a0ec-356e6cbfaad7">

<img width="891" alt="Capture d’écran 2024-05-17 à 17 16 11" src="https://github.com/ultratwo/sybilled20/assets/160050412/04e5f7bc-6481-40ce-af47-a2c5dc187d16">


<img width="905" alt="Capture d’écran 2024-05-17 à 17 14 33" src="https://github.com/ultratwo/sybilled20/assets/160050412/b5731a94-1509-4669-be7f-35c9a808750e">


<img width="889" alt="Capture d’écran 2024-05-17 à 17 14 40" src="https://github.com/ultratwo/sybilled20/assets/160050412/73b3cb06-c610-4a41-aa87-96985d82f43d">

<img width="894" alt="Capture d’écran 2024-05-17 à 17 15 13" src="https://github.com/ultratwo/sybilled20/assets/160050412/8c6c0176-9713-40ec-a585-47cfb7d12364">

<img width="883" alt="Capture d’écran 2024-05-17 à 17 15 36" src="https://github.com/ultratwo/sybilled20/assets/160050412/fea87d9b-6fd9-472d-a0c8-eef32753be70">

<img width="933" alt="Capture d’écran 2024-05-17 à 17 16 03" src="https://github.com/ultratwo/sybilled20/assets/160050412/a87b0d65-4bc0-4ca5-86e2-15954b6a59c7">

<img width="895" alt="Capture d’écran 2024-05-17 à 17 15 46" src="https://github.com/ultratwo/sybilled20/assets/160050412/9b478202-77db-42e3-a39e-816b75f5feac">

<img width="890" alt="Capture d’écran 2024-05-17 à 17 14 55" src="https://github.com/ultratwo/sybilled20/assets/160050412/4d8e5682-4fc2-4334-a122-ce1d42bcd14c">

<img width="897" alt="Capture d’écran 2024-05-17 à 17 15 56" src="https://github.com/ultratwo/sybilled20/assets/160050412/cf0426ea-e6c1-4a2d-ad27-122a5324fc99">


<img width="900" alt="Capture d’écran 2024-05-17 à 17 15 06" src="https://github.com/ultratwo/sybilled20/assets/160050412/da4aa569-f89d-490b-9ad1-062561a3ed7b">


<img width="877" alt="Capture d’écran 2024-05-17 à 17 15 00" src="https://github.com/ultratwo/sybilled20/assets/160050412/904055c4-efe9-4464-91a2-33218e8477ab">


etc...



  
</details>















Another example, ALL the addresses of the cluster locked the same amount of STG on Stargate on the BSC, in a relative similar timespan.









<details>

<img width="647" alt="Capture d’écran 2024-05-17 à 17 23 02" src="https://github.com/ultratwo/sybilled20/assets/160050412/b66afb70-70a7-4a13-b00e-c444db2173b1">

https://bscscan.com/tx/0x1da4d0432260f42690e8ec61afc6a912e906ee408442b58214bcdd3fd5856efc
<img width="631" alt="Capture d’écran 2024-05-17 à 17 23 09" src="https://github.com/ultratwo/sybilled20/assets/160050412/123b6abd-207c-4a2d-990d-8552d8e928ff">
https://bscscan.com/tx/0x6e28990eec739626b1c6a831d57f216a41c1452b447f9a165f8bc256cc7a4551



<img width="640" alt="Capture d’écran 2024-05-17 à 17 23 22" src="https://github.com/ultratwo/sybilled20/assets/160050412/0fc7a4eb-dc14-49a8-88fe-3129be21c519">
https://bscscan.com/tx/0x7263d76239b2b964ab541e12af2e0d6aa1eea89c462b82b3a783cec3f5a9a314
<img width="633" alt="Capture d’écran 2024-05-17 à 17 23 30" src="https://github.com/ultratwo/sybilled20/assets/160050412/d26b7ca4-a93a-4e29-a96d-91670b9a167e">
https://bscscan.com/tx/0x010fb4df8823350726017451ee248f5a4177071a77170cfde318cceae150dd1d

<img width="630" alt="Capture d’écran 2024-05-17 à 17 23 37" src="https://github.com/ultratwo/sybilled20/assets/160050412/c12c35eb-a68a-4b08-b457-387315332f8e">
https://bscscan.com/tx/0x20fc4e7985b557bc0742cbf752196d6a2f9847e408ba71b29491a4b3063e37f1

<img width="633" alt="Capture d’écran 2024-05-17 à 17 23 44" src="https://github.com/ultratwo/sybilled20/assets/160050412/102a0ba8-a0dd-435f-a0ef-3a6ff9bfa15f">
https://bscscan.com/tx/0xb24e3d9cccf1f30b650cbc74fb6bc0aecb145c78670bcbec3142691a4216de62



<img width="649" alt="Capture d’écran 2024-05-17 à 17 23 57" src="https://github.com/ultratwo/sybilled20/assets/160050412/21701ca2-ebde-44b4-93cc-9357d4a53a13">
https://bscscan.com/tx/0x55c17b6baf71bf615527225b4cb9bf5b01e3833f899ff54636f428d972895b82

<img width="660" alt="Capture d’écran 2024-05-17 à 17 24 03" src="https://github.com/ultratwo/sybilled20/assets/160050412/733cb0d2-bbaa-4a06-97df-83e8dc1311b0">
https://bscscan.com/tx/0x05926940525568f333c8ff83ad38f46c01d34448aafac65848f76345a9933f2b

<img width="635" alt="Capture d’écran 2024-05-17 à 17 24 10" src="https://github.com/ultratwo/sybilled20/assets/160050412/9cb0a3f8-b66c-4fa9-acfd-9fddc5aa053c">
https://bscscan.com/tx/0x0a3fdecd05b7b1f1f5f669e2277f03ff4384b92d670ccd782d3134a628c0a9aa


etc...

</details>

Cluster + same cex deposit address + same patterns of transaction to farm airdrops accross the addresses.

