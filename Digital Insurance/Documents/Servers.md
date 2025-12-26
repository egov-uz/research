# Server Related Findings

It was decided that we are going to choose one of following options after the last meeting:

- VDS
- VPS
- VDC
- Colocation


## Product definition

The product is adhere, a digital service provided to either businesses or ordinary customers and the main objective is to create a sort of centralized solution, one single point to purchase insurances legally and is provided by government itself. Product includes basic and core components to function as a web service:

- Backend for data lifting
- Web frontend for browser interface
- Mobile application for more consumer reach

## Why not X?

**VDC** - is considered most loved by businesses and startups for following "pay what you use for" scheme and offers elasticity for the whole infrastructure. Easier to scale compared to statically hosted collocation server. [For more, press the link.](https://info.support.huawei.com/info-finder/encyclopedia/en/VDC.html)

**Colocation** - very pricey at the beginning as server equipments costs few times expensive than usual home/lab/gaming PCs. Also, there's monthly fee of preserving datacenter space. Offers stability and total control over infrastructure, even including hardware  wise. [For more, press the link.](https://en.wikipedia.org/wiki/Colocation_centre)

**VPS** - virtual machine inside a VDC. Elastic space which is bounded to limitations of the host machine itself. Very cheap in terms of maintainance and flexible to the requirements & space. However, raises concerns about privacy as we don't own even the hard drive to preserve ownership over data. [For more, press the link.](https://en.wikipedia.org/wiki/Virtual_private_server)

**VDS** - basically we rent the server as a HaaS and have shared control over hardware (server) between consumer and server provider. However, we won't own the hardware, meaning, as soon as there's an overdue payment fee left behind, there's huge possibility that server providers will reclaim server equipments back without a notice. Also raises privacy concerns in terms of data ownership. [For more, press the link.](https://en.wikipedia.org/wiki/VDS)

The platform that we are going to build is more of data eccentric and does not perform any heavy data processing which requires too much computation power _(a.k.a CPU)_ from servers. **It's more of I/O and network bounded and more focus should be given to these parameters.** Data is the first class citizen in the platform, which means, **any kind of ownership over data should be guaranteed, which eliminates any other options except Colocation**. Speaking of backend software, most backend frameworks tends to queue requests when server can't keep up with the amount of requests incoming, which will hit more RAM as a mean of data preservation. In order to avoid data loss during service, more space in hard storage should be assured to keep up with the amount of data stored in server. Assuming everything above:

> Basically, resource prioritization should be something like this:
> RAM > Hard Storage > CPU

### Real Life Practices

The screenshot below is taken from a server that's running ...

### Options

The following is a suggestion table to serve as a buyer's guide:

|Component   |Low End Specifications|Medium End Specification|High End Specifications|
|------------|:--------------------:|:----------------------:|:---------------------:|
|CPU         | 12 Core +2GHz        | 24 Core +2GHz          | +32 Core +2GHz        |
|RAM         | 32GB DDR4+ ECC m.h   | 64GB DDR4+ ECC m.h     | +128GB DDR4+ ECC m.h  |
|NVME        | 256 GB RAID-1        | 512 GB RAID-4          | +512 GB RAID-4+       |
|SATA        | 4 TB RAID-4          | 4 TB RAID-4            | +40 TB RAID-4+        |

### Reasoning

*Work in progress*

## Colocation Providers

### Hardware Options

This section tries to list all available options whether where to purchase hardware equipments for server deployment.

#### Distributors

During the research, a few server equipment distributors have been found:

- [SevenTrade](https://seventrade.uz/catalog/noutbuki-kompyuternaya-tekhnika/servery/)
- [Servermall](https://servermall.uz/)
- [First](https://first.uz/product/servery/stoechnye-servery-rack/)
- [Asbis](https://catalog.asbis.uz/category/servers)
- [Server Sale](https://sale-server.uz/servery/products)

#### Recommended Options

-

### Colocation Provision

There are few colocation service providers within territory of Uzbekistan.

#### List of distributors

- [Uztelecom](https://uztelecom.uz/ru/chastnym-licam/oblachnye-servisy/colocation)
- [Uzinfocom](https://dc.uz/uzl/page/view?urlname=colocation)
- [Eskiz](https://eskiz.uz/colocation)
- [UzCI](https://www.uzsci.net/Uslugi/Colocation)
- [Comnet](https://comnet.uz/business/colocation)
- [Sarkor](https://www.sarkor.uz/rus/corporate/c_colocation)
