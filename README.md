# junos-checker.py
Juniper设备各种状态自定义监控脚本.Based on the platform of Odin.

基于snmp和pyez两种方式实现
snmp的方式实现以下监控项：
    端口up/down报警
    
pyez的方式实现以下监控项：
    端口光功率：check_chassis_alarms(dev,dev_ip)
    系统报警：check_system_alarms(dev,dev_ip)
    ospf邻居状态报警：check_ospf(dev,dev_ip)
    机框报警：check_chassis_environment(dev,dev_ip)
    系统存储报警：check_system_storage(dev,dev_ip)
    系统coredumps报警：check_system_coredumps(dev,dev_ip)
    dci裸纤故障报警：check_luoxian(dev,dev_ip)
    防火墙连接数报警：check_srx_session(dev,dev_ip)
