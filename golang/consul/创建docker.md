 
 ### consul 实例1
    docker run -itd --name=consule1 -p 8100:8500 --restart=always -e consul_bind_interface='eth0' --privileged=true --name=consul1 consul agent -server -bootstrap-expect=2  -ui -node=consul1 -client='0.0.0.0' -data-dir /consul/data -config-dir /consul/config -datacenter=consul_dc

实例1 ip : 172.17.0.2
### consul 实例2
    docker run -itd --name=consule1 -p 8200:8500 --restart=always -e consul_bind_interface='eth0' --privileged=true --name=consul2 consul agent -server -bootstrap-expect=2  -ui -node=consul2 -client='0.0.0.0' -data-dir /consul/data -config-dir /consul/config -datacenter=consul_dc -join=172.17.0.2