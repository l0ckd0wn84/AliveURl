#!/bin/bash

echo "Enter the website : "
read we_x

status_code=$(curl -s -o /dev/null -w "%{http_code}" $we_x)
echo "The status code is: $status_code"

if [ "$status_code" -eq 200 ]; then
    echo "The web works!"
else
    echo "The web does NOT work."
    exit 1
fi
