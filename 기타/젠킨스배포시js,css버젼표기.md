compile / 배포 이전에 아래와 같이 shell script 수행하여 치환.

find . -type f -name "*.html" -exec sed -i -e s/\\.js\\\"/\\.js?v=${BUILD_NUMBER}\\\"/g {} +
find . -type f -name "*.jsp" -exec sed -i -e s/\\.css\\\"/\\.css?v=${BUILD_NUMBER}\\\"/g {} +
