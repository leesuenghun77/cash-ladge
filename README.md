# cash-ladge
캐시 최대화
# 시스템 캐시 크기 설정
wmic memconfig set MaximumMemoryPercentage=10000
# 시스템 버퍼 크기 설정  
wmic memconfig set MaximumMemoryPercentage=80000
Linux
ini
복사
# sysctl 설정으로 캐시 및 버퍼 크기 조절
sudo sysctl -w vm.swappiness=10000
sudo sysctl -w vm.vfs_cache_pressure=50000
sudo sysctl -w vm.min_free_kbytes=65535000
macOS
ini
복사
# sysctl 설정으로 캐시 및 버퍼 크기 조절
sudo sysctl -w vm.swappiness=10000
sudo sysctl -w vfs.journal.enable=1000
sudo sysctl -w vfs.journal.commit=10000


