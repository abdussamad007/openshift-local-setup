I did set-up the Openshift single node cluster in my local laptop with configuration as attached.

![image](https://github.com/user-attachments/assets/953162cc-2b5c-448b-bb8a-50a68236f826)

Also, Before proceeding I had to enable the virtualization at BIOS level.Otherwise your setup would not work. 
![image](https://github.com/user-attachments/assets/6a823ee9-2097-44d5-b82f-f672611f4e6c)

Once you have your hardwire infra ready - proceed with the installation. I used the steps mentioned here - https://www.redhat.com/en/blog/install-openshift-local
It's simple and easily understandable - just following the steps mentioned can be done easily.

![image](https://github.com/user-attachments/assets/086cbbd5-40a7-4e70-9c95-bcd50b1399fc)

![image](https://github.com/user-attachments/assets/2bc25d10-f97a-4678-855f-31b55a6c8582)

Next I needed secret to start the cluster - Hence I had to download it from here - https://console.redhat.com/openshift/create/local
![image](https://github.com/user-attachments/assets/a441aa23-e2c1-41b8-8adf-aa4633ef48aa)
![image](https://github.com/user-attachments/assets/605991ee-3249-4699-8dfe-b18d5a0f7e60)

If all looks good you would get the below message on console 

INFO Adding crc-admin and crc-developer contexts to kubeconfig... 
Started the OpenShift cluster.

The server is accessible via web console at:
  https://console-openshift-console.apps-crc.testing

Log in as administrator:
  Username: kubeadmin
  Password: LFnM2-F3zb4-dLqsw-HVmLb

Log in as user:
  Username: developer
  Password: developer

Use the 'oc' command line interface:
  $ eval $(crc oc-env)
  $ oc login -u developer https://api.crc.testing:6443
#############################################################################
Now you can use the above webcosole URL and credential to access the via browser.
