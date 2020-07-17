# ddPCR-Poisson-Statistics

#### The purpose of this project is to recreate the Poisson statistics listed in Bio Rad's Droplet Digital PCR Application Guide.

http://www.bio-rad.com/webroot/web/pdf/lsr/literature/Bulletin_6407.pdf

These statistics are shown in Chapter 3: Absolute Quantification and the Statistics of Droplet Digital™ PCR. This was done to show the underlying mathematics of the Poisson distribution.

In probability theory and statistics, the Poisson distribution, named after French mathematician Siméon Denis Poisson, is a discrete probability distribution that expresses the probability of a given number of events occurring in a fixed interval of time or space if these events occur with a known constant mean rate and independently of the time since the last event. The Poisson distribution can also be used for the number of events in other specified intervals such as distance, area or volume. 

## Intermediate Concentration Example - Bio-Rad

Consider the case in which there are 5,000 target molecules in 20,000 droplets (5,000 targets in 20 μl = 250 copies/μl = 0.25 CPD). Random partitioning of target molecules into droplets will lead to some droplets with 2, 3, or even 4 copies, and correspondingly more than 75% of the droplets will have zero copies. Poisson statistics tells us exactly how many droplets to expect in each category. Table 3.1 shows the expected percentage of droplets in each category. Note that in ddPCR, each droplet is distinguished as either empty/negative (zero targets) or occupied/positive (one or more targets). For the 0.25 CPD case, 78% (not 75%) of the droplets will be negative and 22% (not 25%) will be positive on average. Since Poisson statistics arise in multiple different contexts in ddPCR, we describe this phenomenon as “partitioning statistics.

## Advanced Concentration Example - Bio-Rad

Consider the case in which 50,000 target molecules are present in 20 μl (50,000 targets in 20 μl = 2,500 targets/μl = 2.5 CPD). With an average of 2.5 copies of target/droplet, it’s not immediately obvious that there will be any empty droplets. But Poisson statistics predicts that there will be some empty droplets (1,642 empty droplets) and gives a precise relationship between the average number of copies/droplet and the expected fraction of empty droplets. Table 3.2 shows how many droplets we expect to see with 0, 1, 2, 3, 4, or more copies/droplet when there are on average 2.5 copies of target/droplet, or 50,000 copies in a 20 μl reaction volume.
