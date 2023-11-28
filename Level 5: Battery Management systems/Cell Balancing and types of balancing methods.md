In the previous chapters, we have seen how different cells in a battery can become unbalanced over time and would in turn cause numerous safety concerns.

Let's now look at how a battery management system prevents cell imbalance, and also different methods a BMS uses to charge and stabilize an in-balanced battery pack.

https://do7js0tdxrds1.cloudfront.net/r0awma771e8tr0v7f6jfdbbl1bav?response-content-disposition=inline%3B+filename%3D%22Skizze_Balancer.png%22%3B&response-content-type=image%2Fpng&Expires=1701167711&Signature=XDvt7-WbL-GJ~rc~tmqYkZRC3ybwFK3cdeAdEUXRUPo0KirScpKiJFt-AEowbIuXNtWK6qndtXHspen-rswIYAclO33fTQmV4dYXFgXOJ7eIeqFJWCkO6qDZuM7~rszfD5gHX7mAdVwRK7TrETILXc1SQONzC4rJb5q2nrqOAQ8BSAD-hSlk6LKAKR2A8rvp3NSCJ-~ExmbDiFxmcFZBZ-2SlgrpKhnugbT9ZF4A~MKtLmhRxSqwp-~JAyfn3hzTokjTmlsSHuuEMBF0~0xnH6qTj8CRxrmiOIjDi56sQDjXfBMzIB2YwJIp6-xtz7SjBd0Q2ON6oEsK~GWxQBrtXw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

-=- Different ways cells are imbalanced
-=- *Source: [Hadhuey](https://commons.wikimedia.org/wiki/File:Skizze_Balancer.png) | License [(CC BY-SA 3.0)](https://creativecommons.org/licenses/by-sa/3.0/deed.en)*

There are 2 different balancing algorithms utilized by BMS systems. These are

1. Passive Balancing
2. Active Balancing

https://do7js0tdxrds1.cloudfront.net/gjhre2ya490wyzp655m5d18x02r0?response-content-disposition=inline%3B+filename%3D%22Cell+balancing.png%22%3B&response-content-type=image%2Fpng&Expires=1701167711&Signature=s~m8k7LDXH2DBw0wsiCKb3CHD0O9ZAmeqgXlz7fSRuqvXXMOf5JUcP33~XKZ-DrQBH6LdYdXSMR5SiKrfpviooC~BbXbqeElnl1xlGJhUKudxqKFyESPHWtLyGGDUljp0VZEz6QikYs0tQzjedmE0xK5xX1MLhLYmHgn1cas8uZQP3LACgR2PsLq5qzzuzXzKOqi7xQwhX-LI4Y93yO0nFgDBbqUjdhBFKbdWNtxwIb64smhsKmZ8229H0ujawnIUfRgaFW4PFzmtmhAdpGXE7XQGokB0C-HTFD5T1EDfImR5mNnJfxWBUWNaJV98M5MPWVZLw3HS5ym0PUHz0UYvg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Types of Cell Balancing Methods

# 1. Passive balancing

Passive balancing drains charge from cells having too much
charge and dissipates drained energy as heat.

For example, if a cell in a battery pack is overcharged by a bit, the battery management system will isolate that individual overcharged cell and route it in such a way that the terminals are connected to a resistance. This will make the current start flowing through the resistor and will reduce the charge in that particular overcharged cell. 

There are 2 ways to passively balance a cell.

1. Fixed shunt resistor
2. Switched shunt resistor

### 1. Fixed Shunt Resistor (Passive balancing)

https://do7js0tdxrds1.cloudfront.net/a7g7927p34mco203377d0rmawwij?response-content-disposition=inline%3B+filename%3D%22fixed+shunt+resistor.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167711&Signature=M3myQVJkxNcr9CktXf3zbkBCXZBEQ8R7F-CFCbKkooZE7N6zX8hpuPwPqCwK8rgjyT91jrz0UPnfpIkbU6Mrqip7LLGUjNvn3bbKyPeRbm0E6OPFVReZpd~o50pZpBqVA2KKNjhxVsQOeYB3TDTMZ29YBQnPLlsGOGJxcCNblFLsP-RAak7BTvmSXpWTQSnWA8vnHpPatWlqyJr06kjgCuzlblZ4D6pYrWYHMsEKuSmQZNyDTVGO5qdAeWd601KbrZTpzxAZ~Sn2r70Zpi9Mh92Bb1r5vE6vkmzvlkEpgh1beDkubn3c-Xj2jRBLWEbGUF3F8byUSIjWoeZMdxWVcQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Fig 1 : Fixed Shunt resistor


In this particular balancing method, the general idea is that a resistor is placed in parallel with each cell,
and used to drain charge from that cell. The energy removed from the cell is dissipated as heat.

As you can see from Fig 1, the circuitry is simple. It basically works on the idea that high-voltage cells will have a greater discharge rate,
and thus will self-discharge more quickly than low-voltage cells and get balanced from the resistors.

> Note that the circuit is always dissipating charge, even when the pack is perfectly balanced.

As a solution to this problem, we can add Zener diodes to "Shut off" balancing when cell voltage drops below some voltage point.

https://do7js0tdxrds1.cloudfront.net/85uggktss7bfs57a1yt5jrk6emfv?response-content-disposition=inline%3B+filename%3D%22fixed+shunt+resistor+with+zener.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167711&Signature=oTKlI~ZMpQBfreGo571UFcbzP2Z0t1ENN~hashcCR13ZtTVkOLdBxTRF8c-bjhOFoNrcilUIwNYEBoMy8abuy8lPqT6hJi~R7VGbYec7LcKdMzLmr5N3afxGFs0HlwhpMOTx2Zi7TKQHSMsnvOWXuwe-80WEQeYfiwYEpTK3FvUJGzIPTpZ8WJ7-ui4p3xiHU-oJ-VWOBnAIG4nd9Sv6r6Qq-5Y1M6OvoJ3ezD5rygZ-Z~loEbjWYDPLQAgwIcN1TLI3OOM8vn9NkfzRkFcpIVg1v83SrSCochhrzotk0KFWPp2679i6o3F0nDJf6PNG8V~fq2ESRj5Xc0-HFxotfQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Fig 2 : Fixed Shunt resistor with Zener diodes


When a cell’s voltage is above the Zener setpoint, the resistor path is
activated, and that particular cell’s charge is depleted until the cell’s
voltage drops below the Zener setpoint.

Note that this design works for chemistries where overcharge is
tolerable, and the cell can “float”.

>Float means to be able to overcharge and stay in that condition over long periods of time. 

Usually, Li-ion batteries do not tolerate overcharge voltages, and thus this method is not advisable.

### 2. Switched Shunt Resistor (Passive balancing)

This is a variation of fixed shunt resistor design, where the Zener diode circuit is replaced with a microcontroller controlled switch

The switch can be a transistor circuit or a relay-based circuit.
https://do7js0tdxrds1.cloudfront.net/u8usyz28xyq8vf7fucntljbf9cr4?response-content-disposition=inline%3B+filename%3D%22switched+shunt+resistor.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167711&Signature=gH2L-8ffg3DD2p-w8-6kKFAZBty22XlknnVBFS4VH8fFEtPHURuzPJe5~mmEsq6Z4Ujyb0yuqdqGH6suIMoBd4z~4nGRTu1C~HEdcKa6ipUTUMF31sq1XxgJhez3xu75R09p6SXvC-ckuxzRAwcFeHd3AHkEvjJ56N00FumRelYAgOfSgc~NjsAoiObTBglA8-szL69QfWSjgVB6XxldipkDy84c5Y~-R8W4xFMYYJb6dEyTot4wWsciVAZJz8SzOFlJRmI5hwlCsv21MYJp6337sRRCQgrrPJQt-w92D7WbpKTBuOljFAvBviSskF8s6jsTKi26gH~rCsBbALCexw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Fig 3 : switched shunt resistors

In this design, the BMS or the microcontroller closes switches on cells having too much charge, allowing them to drain via the resistors.

The primary advantage of these types of passive balancing is
the simplicity (and hence, lower cost) of the circuitry involved,
compared with active balancing designs.

### The Drawbacks of passive balancing are:

1. Energy is wasted as heat, which could be otherwise used
productively.

2. The quantity of heat generated by balancing can be comparable
to the heat generated by normal cell operation. This may also increase the cooling requirements for the battery-pack thermal management system, which is a significant expense.

3. Battery pack life could be shorter than a pack which has an active balancing design.
   * Pack life is determined by the weakest cell in the pack.
   * The active balancing can use strong cells to support weak cells,
bringing the pack to a uniform end-of-life configuration.
--------------

# 2. Active Balancing

Active balancing circuits break down into three general categories:
* Move charge via switched capacitors
* Move energy via transformer/inductor designs

In short, unlike passive balancing where cells with a higher charge than normal are discharged by connecting them to resistance and discharging their extra charge by generating heat, Active balancers transfer the extra charge from overcharged cells to undercharged cells. Thus, there is no energy wasted.

Let's have a look at an example circuit of an active balancer below in Fig 4,

https://do7js0tdxrds1.cloudfront.net/3zhmz3hnk8zb6mnzzci4l7dq7dy3?response-content-disposition=inline%3B+filename%3D%22Multiple+switched+capacitors.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167711&Signature=JFxl9vUEWTPDveSzZdQ2JtfqBct1D97Nf55vPRfCRUmndeg0IcCt4hnGTheWxyN1AF2qSfB0Bt1BFpo5hrAHkDDYJgMjz1SKw0fK1ERBdY703E1XuzAWCRvyiOKjN3LxgsI~0s0t64vX79t64KSt8PpPR62R02JEmHBpICSoGUrogI2yKDPD6H9YnoPHHnHVKc84qM11uEpie1yg3sknIoDLSpGS8ZBIgCnxFXzzgAJ-0oev~3yg1NW1pZKntu2rQLfOmGIe5vv23bemT8waQE8rNeIWbyiVCQzhfT7ExeeZTBccAggxZyAQ~MVcSWC5qLB5uStzy2T0dkW91PdjMQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Fig: 4

Consider two neighboring cells. The higher-voltage cell charges the
capacitor to its voltage, and then the lower-voltage cell discharges the
capacitor to its voltage, thus the charge moves to equalize cell voltages.

Over the course of time, the entire battery pack can be equalized. But, the charge takes a long time to propagate from one end of the
pack to the other.

Let's take a look at the different types of active cell balancers:

### 1. One switched capacitor (Active)

This design utilizes a single capacitor with an intelligent control module for the switches, unlike the circuit in fig 4 where multiple capacitors are used.

https://do7js0tdxrds1.cloudfront.net/cnvuvb110putvzxqajstmkmxjib4?response-content-disposition=inline%3B+filename%3D%22one+switched+capacitor.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167711&Signature=PPVIv53r7164tBmA0Vh-xT1HgdnlFcGecQVVfGd~Wrk4TrL8gwjKbHcxXzqyCzB3gdGPeXjWJVaLcgkrmKFaqgZK1PzT5PZ274exlKiUAlyHgUWYvD~mcyZ-NFxU4cI7R30NADXrYYkE4c0GLI5zMQKk~KBbHNZMaqaJNkyRy2YS3c-g3Zz8wYfP0NSr5M3NbQh2PD5HPTfmndwbOM3XP93vaWOHJLeK895~vCyfDkc9sXVUxGjVGgJ8vJdToYGwsOZwH3e~j8L9yhb4JeShV5YvFki1oVovcJHFQ7BiulIm1xLPVvEQfcHTAkploovirtHD2KYRQ4pzD5ZFncS~vQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Captions: Fig 5: One switched capacitor

This method allows direct movement of charge from a high-voltage to a
low-voltage cell.

* But a serious drawback of all capacitor-based designs is that they rely on
a voltage difference between cells to work.

* Most lithium-ion chemistries have very little voltage variation between
cells even if SOC varies a lot.

* Capacitor-based designs make the most sense for EV, where voltage
variation can be fairly large.
------------

There are 3 more Active balancing methods, namely,
* Shared transformer Method
* Switched transformer Method
* Shared bus Method

We will not be discussing these methods as these will turn out to be very complicated for the course. Therefore, we will be moving on to building our own BMS for a lead-acid battery pack in the next upcoming chapters.