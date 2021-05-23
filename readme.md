apt-get update
apt-get install vim

occ app:install documentserver_community
 occ app:install onlyoffice

docker run --rm -it --name dcv -v $(pwd):/input pmsipilot/docker-compose-viz render -m image docker-compose.yml
# PowerShell
docker run --rm -it --name dcv -v ${pwd}:/input pmsipilot/docker-compose-viz render -m image docker-compose.yml

'user_backends' => array(
    array(
        'class' => '\OCA\User_External\WebDAVAuth',
        'arguments' => array('https://example.com/webdav'),
    ),
),


curl  -H "OCS-APIRequest: true" \
  http://zzz:AAA123123aaa@localhost/ocs/v2.php/apps/external/api/v1
