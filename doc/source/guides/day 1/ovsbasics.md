##Check bridge flows
- `ip a` --> to list the bridges
- `ovs-ofctl` --> OpenFlow switch management utility
- `ovs-ofctl show br-int` --> show OpenFlow flows for br-int
- `ovs-ofctl dump-flows br-int table=0` --> shows the flow information for the first OF table. The `resubmit` action allows you to follow the flow of the frames 

