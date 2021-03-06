# Overview
To allow for auto-discovery of a microservice it must be registered with Zookeeper.

## Configuration
The Zookeeper properties must be configured in the `parameters.config` file located in `etc` of the microservice.

Set the announcement point of the microservice.
    
    -com.deciphernow.server.config.zk.announcementPoint=/some/service/endpoint
    
Set the Zookeeper server/port locations. If more than one Zookeeper use a comma to separate them.
    
    -com.deciphernow.server.config.zk.zookeeperConnection=zookeeper-01:2181,zookeeper-02:2181,...,zookeeper-0N:2181
    
## Register IP address
If for whatever reason the IP address is preferred over the hostname when registering the microservice with Zookeeper then follow these [instructions](ConfigureIPAddressResolution.md) 
