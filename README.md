# kaspa
# create a swap memory by taking a new disk of 50gb, increase swappiness to 10 so that indexer contaiuner uses swap more readily instead of caching/buffering the ram heavily. postgres gets killed if there is no swap memory
# use below commands:
#  sudo sysctl vm.swappiness=10
#  echo 'vm.swappiness=10' | sudo tee -a /etc/sysctl.conf
#Thenn run compose file with custom postgres file in place
