# VM_Cluster
Hyper-V

Failover cluster is a feature to provide available VM, if a node on which a VM is running fails, then the failover cluster will "restart the VM automatically" on a different node.

![failover cluster](https://i0.wp.com/www.itpromentor.com/wp-content/uploads/2016/12/hv-cluster-3.png?w=1560&ssl=1)

# Components of Failover Cluster



                    shared bus || iSCSI connection
                                |                  \
                                |                   \        Failover Cluster
                                V                    \
          Node1(Host/Server) ------ Cluster Storage ------- Node2(Host/Server)
         |           |                                               |          |
         |           |                                               |          |
         |           |______a dedicate network connects the nodes____|          |
         |                                                                      |
         |__________________________Clients_____________________________________|
                   ( a network connects the failover clusters and clients)          

- [x] SMB, Server Msg Block.

- [x] iSCSI, to config Internet Small Computer Sys Interface.

- [x] Virtual Hard Disk, to present shared storage to VMs.

they can provide high availability, and share storage.

* Quorum

* Encryption for Cluster Shared Volumes.

# Main Roles in Failover Cluster

(1) Shared Storage, 叢集共享記憶體

(2) iSCSI Connection, 叢集網路介面

(3) Encrpted Custer Volume, 加密的叢集卷宗



