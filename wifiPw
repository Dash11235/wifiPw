#!/bin/bash

cd /etc/NetworkManager/system-connections

for i in $(ls); do
    for j in $(sudo cat $i); do
        if [[ $j = id* ]]
        then
            echo -n "$j,"
        elif [[ $j == psk* ]]
        then
            echo " $j"
        fi
    done
done
