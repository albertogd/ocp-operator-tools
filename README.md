# OCP Operator Tools
Repository of operator tools for Openshift 

## getOperatorImages
Retrieve all the related images of an operator. This is useful to get the image list to pull for disconnected environments.

Example: Get all the related images of 

    $ ./getOperatorImages ansible-automation-platform-operator 2.2.0+0.1660690990
    registry.redhat.io/ansible-automation-platform-22/ee-minimal-rhel8@sha256:5af0d5320c797103ac34aaa33620c12dfdff7fcdcb9a96b2eb1e2bb34afb91b0
    registry.redhat.io/ansible-automation-platform-22/controller-rhel8@sha256:0f254deb891bf69dd92d766ba8e73b14effd008fbac97dd4299441e9401a44c8
    registry.redhat.io/rhel8/postgresql-13@sha256:cf0c33620cf579c7fb25e7787c1e73cc916becf3e33b7f5f52912a49a00c47a8
    registry.redhat.io/ansible-automation-platform-22/ee-29-rhel8@sha256:706310befe132fef2288e2e16b6f59ab35cf829d108bd575ab80da96054ae6f6
    registry.redhat.io/openshift4/ose-kube-rbac-proxy@sha256:260ebab52c1e825e354bfa60827e314388fb7878bfa16d1dc061707962e95bea
    registry.redhat.io/ansible-automation-platform-22/platform-resource-rhel8-operator@sha256:802a7134d71939f643b9558d0e7a193c2e72cef6fa300011e5a5051da90bc166
    registry.redhat.io/ansible-automation-platform-22/hub-rhel8@sha256:69a80384a5f2e8d8ab71c7537fba087c57a24b84a4f0088a3c7c69a97e437ed0
    registry.redhat.io/ansible-automation-platform-22/ee-supported-rhel8@sha256:f1bd44cb3aff459f05af7855f0bcea8a0d7a44c85acd6d0f2c64148d137502e8
    registry.redhat.io/ansible-automation-platform-22/hub-web-rhel8@sha256:5329479ebe031fdff81ca600dd1fd1a876edec1c7e90d4c282d4aac5727bf081
    registry.redhat.io/ubi8/ubi-minimal@sha256:c536d4c63253318fdfc1db499f8f4bb0881db7fbd6f3d1554b4d54c812f85cc7
    registry.redhat.io/rhel8/redis-6@sha256:d7c7852338717308cbb59e9303e1ea35cc8e5c01ceb2818569be20c15f3f943d
    registry.redhat.io/ansible-automation-platform-22/platform-resource-runner-rhel8@sha256:006451baa500bc588bba0499f489b2cb3c145e75a016304a20a3e3e194f675e6
    registry.redhat.io/ansible-automation-platform-22/controller-rhel8-operator@sha256:e1a939e28005f6d7ee95754599495312ae58b3da0f375bc18962e6f7b00d4676
    registry.redhat.io/ansible-automation-platform-22/hub-rhel8-operator@sha256:88d20e394baee456df73f3c35f3866b9dd658c5ca585f4cb33a7dcafd0ca63e3

## getACMimages
Retrieve all the related images of ACM operator. This is useful to get the image list to pull for disconnected environments. The output will show different sections for Agent images, ACM images and MCE images.

    $ ./getACMimages.sh 2.6.0 2.1.0
    <<< START LIST OF ACM AGENT IMAGES >>>
    registry.redhat.io/rhacm2/cert-policy-controller-rhel8@sha256:09ddf46ce8fdb73fa1e71acbbd9852d2082c6521984aff37778365e5fa4ec7e8
    registry.redhat.io/rhacm2/config-policy-controller-rhel8@sha256:e651d5d18a06b18de8b927f2c51e17a422b69a667858ed23c52731d3481a5df4
    registry.redhat.io/rhacm2/governance-policy-status-sync-rhel8@sha256:1191a0086b90ca39f54223b23b6204e7597ae5ab2dcbfdb4ef04e34225d10628
    ...
    <<< END LIST OF ACM AGENT IMAGES >>>


    <<< START LIST OF ACM OPERATOR 2.6.0 IMAGES >>>
    registry.redhat.io/rhacm2/klusterlet-addon-controller-rhel8@sha256:89b645247ac589bf7a906380fc81567b2a26bdb743742bffa33fde82a6a2761b
    registry.redhat.io/rhacm2/governance-policy-status-sync-rhel8@sha256:1191a0086b90ca39f54223b23b6204e7597ae5ab2dcbfdb4ef04e34225d10628
    registry.redhat.io/openshift4/ose-oauth-proxy@sha256:7b752f852e890fab8e74aac70c0f3f4fea6959676c15f2314a7f8252d37c90f2
    ...
    <<< END LIST OF ACM OPERATOR 2.6.0 IMAGES >>>


    <<< START LIST OF MCE OPERATOR 2.1.0 IMAGES >>>
    registry.redhat.io/multicluster-engine/hypershift-deployment-controller-rhel8@sha256:53f86494afb4b0771acfd765747f423d38bc23c4d6a68d40343f6d4270020c2a
    registry.redhat.io/multicluster-engine/cluster-api-rhel8@sha256:9c2cf8542355440d2bb85cad6d43d7be21c042c570fd55867ea2efe8a41116bf
    registry.redhat.io/multicluster-engine/apiserver-network-proxy-rhel8@sha256:2c0f040c004ff7725d56fccb45341874ade16dd3832b28ef9cc82d8dd118afe6
    ...
    <<< END LIST OF MCE OPERATOR 2.1.0 IMAGES >>>



