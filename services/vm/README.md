# Libcloud objbects returned by clouds

## AWS



```
{'_uuid': None,
 'created_at': datetime.datetime(2018, 11, 9, 16, 44, 4, tzinfo=<libcloud.utils.iso8601.Utc object at 0x1038ffe80>),
 'driver': <libcloud.compute.drivers.ec2.EC2NodeDriver object at 0x10250c588>,
 'extra': {'architecture': 'x86_64',
           'availability': 'us-west-2a',
           'block_device_mapping': [{'device_name': '/dev/sda1',
                                     'ebs': {'attach_time': datetime.datetime(2018, 10, 25, 19, 0, tzinfo=<libcloud.utils.iso8601.Utc object at 0x1038ffe80>),
                                             'delete': 'true',
                                             'status': 'attached',
                                             'volume_id': 'vol-0081afab5b6fbe25a'}}],
           'client_token': '',
           'dns_name': 'ec2-52-89-23-7.us-west-2.compute.amazonaws.com',
           'ebs_optimized': 'false',
           'groups': [{'group_id': 'sg-1f8ae364',
                       'group_name': 'launch-wizard-2'}],
           'hypervisor': 'xen',
           'iam_profile': None,
           'image_id': 'ami-0bbe6b35405ecebdb',
           'instance_id': 'i-0fad7e92ffea8b345',
           'instance_lifecycle': None,
           'instance_tenancy': 'default',
           'instance_type': 't2.micro',
           'kernel_id': None,
           'key_name': 'ec2',
           'launch_index': 0,
           'launch_time': '2018-11-09T16:44:04.000Z',
           'monitoring': 'disabled',
           'network_interfaces': [<EC2NetworkInterface: id=eni-0dfc8e30289e6aa34, name=eni-0dfc8e30289e6aa34],
           'platform': None,
           'private_dns': 'ip-172-31-28-147.us-west-2.compute.internal',
           'product_codes': [],
           'ramdisk_id': None,
           'reason': '',
           'root_device_name': '/dev/sda1',
           'root_device_type': 'ebs',
           'source_dest_check': 'true',
           'status': 'running',
           'subnet_id': 'subnet-219fd246',
           'tags': {'Name': 'p1'},
           'virtualization_type': 'hvm',
           'vpc_id': 'vpc-52182935'},
 'id': 'i-0fad7e92ffea8b345',
 'image': None,
 'name': 'p1',
 'private_ips': ['172.31.28.147'],
 'public_ips': ['52.89.23.7'],
 'size': None,
 'state': 'running'}
 ```
 
 ## Azure
 
 ```
 {'_uuid': None,
 'created_at': None,
 'driver': <libcloud.compute.drivers.azure_arm.AzureNodeDriver object at 0x10f974668>,
 'extra': {'id': '/subscriptions/00000a00-00aaa-000a-00aa-000ab00a0000/resourceGroups/CLOUDMESH/providers/Microsoft.Compute/virtualMachines/cm-test-vm-1',
           'location': 'northcentralus',
           'name': 'cm-test-vm-1',
           'properties': {'hardwareProfile': {'vmSize': 'Basic_A0'},
                          'networkProfile': {'networkInterfaces': [{'id': '/subscriptions/00000a00-00aaa-000a-00aa-000ab00a0000/resourceGroups/cloudmesh/providers/Microsoft.Network/networkInterfaces/cm-test-vm-1-nic'}]},
                          'osProfile': {'adminUsername': 'azureuser',
                                        'computerName': 'cm-test-vm-1',
                                        'linuxConfiguration': {'disablePasswordAuthentication': True,
                                                               'ssh': {'publicKeys': [{'keyData': 'ssh-rsa '
                                                                                                  'bbbb...'
                                                                                                  'user@iu.edu',
                                                                                       'path': '/home/azureuser/.ssh/authorized_keys'}]}},
                                        'secrets': []},
                          'provisioningState': 'Succeeded',
                          'storageProfile': {'dataDisks': [],
                                             'imageReference': {'offer': 'UbuntuServer',
                                                                'publisher': 'Canonical',
                                                                'sku': '16.04-LTS',
                                                                'version': 'latest'},
                                             'osDisk': {'caching': 'ReadWrite',
                                                        'createOption': 'FromImage',
                                                        'diskSizeGB': 30,
                                                        'name': 'cm-test-vm-1',
                                                        'osType': 'Linux'}},
                          'vmId': '995784f1-e5b5-4eaa-8fa1-8bfa84386a2d'},
           'tags': {},
           'type': 'Microsoft.Compute/virtualMachines'},
 'id': '/subscriptions/00000a00-00aaa-000a-00aa-000ab00a0000/resourceGroups/CLOUDMESH/providers/Microsoft.Compute/virtualMachines/cm-test-vm-1',
 'image': None,
 'name': 'cm-test-vm-1',
 'private_ips': ['10.0.0.4'],
 'public_ips': ['65.52.27.42'],
 'size': None,
 'state': 'running'}
 ```

## Openstack - Chameleon
``` 
{'_uuid': 'fffa36312f28102732d63f2fbddc50db36d2ae92',
 'created_at': datetime.datetime(2018, 11, 8, 20, 44, 22, tzinfo=<libcloud.utils.iso8601.Utc object at 0x0000021AE543CDA0>),
 'driver': <libcloud.compute.drivers.openstack.OpenStack_1_1_NodeDriver at 0x21ae9c12908>,
 'extra': {'access_ip': '',
  'access_ipv6': '',
  'addresses': {'CH-819337-net': [{'OS-EXT-IPS-MAC:mac_addr': 'fa:16:3e:64:73:6c',
     'OS-EXT-IPS:type': 'fixed',
     'addr': '192.168.0.132',
     'version': 4}]},
  'availability_zone': 'nova',
  'config_drive': '',
  'created': '2018-11-08T20:44:22Z',
  'disk_config': 'MANUAL',
  'fault': None,
  'flavorId': '2',
  'hostId': 'a07787dc6544246e5e284c308b1847e80e45e8264f7ba9ed89d62fd5',
  'imageId': '0b261cb9-e9ab-4f38-8988-1ccc71f9c070',
  'key_name': None,
  'metadata': {},
  'password': None,
  'power_state': 1,
  'progress': 0,
  'service_name': 'nova',
  'task_state': None,
  'tenantId': 'CH-819337',
  'updated': '2018-11-09T17:09:45Z',
  'uri': 'http://openstack.tacc.chameleoncloud.org:8774/v2/CH-819337/servers/9bca2334-cac8-4cbd-bcdd-7af00f6345dc',
  'userId': 'TBD' , # will be replaced by actual user name
  'vm_state': 'active',
  'volumes_attached': []},
 'id': '9bca2334-cac8-4cbd-bcdd-7af00f6345dc',
 'image': None,
 'name': 'cm_test',
 'private_ips': ['192.168.0.132'],
 'public_ips': [],
 'size': None,
 'state': 'running'}
```
