# Copyright 2015-present Facebook. All Rights Reserved.
lib: libfby2_sensor.so

libfby2_sensor.so: fby2_sensor.c
	$(CC) $(CFLAGS) -fPIC -c -o fby2_sensor.o fby2_sensor.c
	$(CC) -lm -lbic -lipmi -lipmb -lfby2_common -shared -o libfby2_sensor.so fby2_sensor.o -lc

.PHONY: clean

clean:
	rm -rf *.o libfby2_sensor.so
