**Pulse Dx**
cat sales_order_item.txt | C:\kafka\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9094 --topic operational-salesorderitems --compression-codec zstd

**Component Context**
cat .\allocation-1.txt | C:\kafka\bin\windows\kafka-console-producer.bat --bootstrap-server localhost:9092 --topic operational-allocation --compression-codec zstd
