=======================================================================
Provision CLOS fabric using Dell EMC Networking Ansible modules example
=======================================================================

This example describes how to use Ansible to build a CLOS fabric with Dell EMC Networking OS10 switches. The sample topology is a two-tier CLOS fabric with two spines and four leafs connected as mesh. EBGP is running between the two tiers.

All switches in spine have the same AS number, and each leaf switch has a unique AS number. All AS number used are private. For application load-balancing purposes, the same prefix is advertised from multiple leaf switches and uses *BGP multipath relax* feature.


