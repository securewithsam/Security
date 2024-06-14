### Linux Batch File 

```sh
sudo yum install cifs-utils
```
![image](https://github.com/securewithsam/Security/assets/85324643/57ea4a2a-0c91-4fd6-869e-a203dcea7c48)

```sh
sudo nano ~/.ciscredentials
```
![image](https://github.com/securewithsam/Security/assets/85324643/bbbe2d5c-9f1e-4f24-9ce5-0130f47f1358)

```sh
nano /etc/fstab
```
```sh
# Added for remote ccpd script run from mvp-infcis-01
//sws-infcis-01.sws.corp/cis /mnt/cis cifs credentials=/root/.ciscredentials 0 0
```
![image](https://github.com/securewithsam/Security/assets/85324643/2f742056-127c-44a5-8aab-1dab7f8f5edd)
```sh
sudo mount /mnt/cis
cd /mnt/cis/Assessor-Linux
sudo ./cis-cat-centralized-ccpd.sh
```

![image](https://github.com/securewithsam/Security/assets/85324643/d07e06d9-451b-442a-88d1-eb0e5fed2090)
