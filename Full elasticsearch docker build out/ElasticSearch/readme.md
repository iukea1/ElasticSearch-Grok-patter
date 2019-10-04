

X-pack Auth
-----------
- To set the default passwords for the default user accounts 
  - example: elastic
Navigate to the filepath below in the docker container

```
bin/elasticsearch-setup-passwords interactive
```

NetFlow 
-----------
Port numbers 
**Logstash** The UDP port on which to listen for Netflow messages	2055

**Logstash**The UDP port on which to listen for sFlow messages

**Logstash**The port on which to listen for IPFIX messages via TCP	4739

**Logstash**The port on which to listen for IPFIX messages via UDP	4739


Netflow index names

```
elastiflow-3.5.1-%{+YYYY.MM.dd}
```

Netflow fields 
-----------
```
   "@timestamp",
          "@version",
          "event.host",
          "event.type",
          "flow.application",
          "flow.autonomous_system",
          "flow.bgp_next_hop",
          "flow.bgp_valid_state",
          "flow.city",
          "flow.country",
          "flow.country_code",
          "flow.direction",
          "flow.dst_addr",
          "flow.dst_addr_trans",
          "flow.dst_asn",
          "flow.dst_hostname",
          "flow.dst_mac",
          "flow.dst_mask_len",
          "flow.dst_port",
          "flow.dst_port_trans",
          "flow.dst_port_name",
          "flow.input_ifname",
          "flow.input_snmp",
          "flow.ip_protocol",
          "flow.ip_version",
          "flow.next_hop",
          "flow.output_ifname",
          "flow.output_snmp",
          "flow.rep_tags",
          "flow.sampling_interval",
          "flow.service_name",
          "flow.src_addr",
          "flow.src_addr_trans",
          "flow.src_asn",
          "flow.src_hostname",
          "flow.src_mac",
          "flow.src_mask_len",
          "flow.src_port",
          "flow.src_port_trans",
          "flow.src_port_name",
          "flow.tcp_flags",
          "flow.tos",
          "flow.traffic_direction",
          "flow.traffic_locality",
          "flow.vlan",
          "node.ipaddr",
          "node.hostname",
          "tags"
```