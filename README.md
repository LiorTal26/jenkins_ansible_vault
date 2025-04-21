# jenkins-example-ansible

if u are using jenkins on container u need to install ansible 
check if the jenkins have ssh key for the machines 

then run the code using jenkinsfile-1 with jenkins pipeline

jenkins blue green

 ansible-playbook -i inventory.ini playbook.yml \
                                      --extra-vars "nginx_port=${NGINX_PORT_SECRET} headers_name=${NGINX_HEADERS_SECRET} jenkins_build_number=${JENKINS_BUILD_NUMBER}" \