CC = gcc
CFLAGS = -C -Wall -I$(PWD)/../../../host_common/include/ -I$(PWD)/../../../../common/protobuf-c/ -I$(PWD)/../../../../common/include/
TARGET = test.out

PWD := $(shell pwd)

all:
	$(CC) $(CFLAGS) $(PWD)/../../../../common/protobuf-c/protobuf-c/protobuf-c.c $(PWD)/platform_wrapper.c $(PWD)/../../../../common/esp_hosted_config.pb-c.c $(PWD)/../../../host_common/transport_pserial.c $(PWD)/../../../host_common/commands.c test.c -o $(TARGET)

clean:
	rm -f $(TARGET) *.o
