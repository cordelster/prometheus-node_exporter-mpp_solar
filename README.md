# prometheus-node_exporter-mpp_solar
Allows collection of data from solar inverters and providing the data directly to prometheous via Prometheus node_exporter and mpp_solar.

### Requires:
* Prometheus node_exporter
* python mpp_solar https://github.com/jblance/mpp-solar

### switching gears here for the one that is watching. Code submission sent up stream to the mpp_solar project now has prometheus node_exporter output. mpp-solar -o prom -- getstatus

submittal of code upstream for mpp_solar to be capable of output in the form of node_exporter was the proper way to go about the objective. 

grafana dashboard and instructions are in the pull request for mpp_Solar for John's review at the time of this writing.

I'm changing the direction to either create a true exporter or maybe just a installer script for those that are not so code gifted.

I also have a turnkey linux builder that builds up grafana and your choice of tdb that I may add this as an option. basicly builds an enterprise setup for you in 10 minutes. if you're not familiar with turnkey linux, it allows a purpose built detain based system that is available as either an .iso image, ova for VMware,  or lxc for proxmox/kvm.

another option is since raspberry Pis availability is getting better, I can create a pi based OS that's  not as susceptible to corruptions and uses two USB drives as a mirrored data set.

open to discussing.

cheers 
