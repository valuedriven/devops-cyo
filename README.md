## TODO
https://docs.ansible.com/ansible/latest/collections/amazon/aws/aws_ec2_inventory.html


apt-get install python3-venv
python3 -m venv ansible
source ansible/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install ansible==2.10
python3 -m pip install boto3 botocore

apt install virtualenv
virtualenv -p /usr/bin/python3 py3
source py3/bin/activate
pip install boto3 botocore ansible==2.10
pip install ansible==2.10
export ANSIBLE_PYTHON_INTERPRETER=$VIRTUAL_ENV/bin/python3

sudo ansible-playbook -vvvvv ambiente/create-keys.yml --extra-vars 'ansible_python_interpreter=/usr/bin/python3'