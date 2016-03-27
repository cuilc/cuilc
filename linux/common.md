#!/bin/env bash

echo "show ip in range 131 to 136"
for ip in 192.168.1.13{1..6};do echo $ip;done

echo "generate sequence from 1 to 10 by step 2"
seq 1 2 10
