# To install pip in linux machine
    [vagrant@linux ~]$ sudo yum install python-pip
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
     * base: mirror.fileplanet.com
     * epel: d2lzkl7pfhq30w.cloudfront.net
     * extras: mirror.ilumno.com
     * updates: mirror.team-cymru.com
    Resolving Dependencies
    --> Running transaction check
    ---> Package python2-pip.noarch 0:8.1.2-10.el7 will be installed
    --> Processing Dependency: python-setuptools for package: python2-pip-8.1.2-10.el7.noarch
    --> Running transaction check
    ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    --> Running transaction check
    ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    --> Running transaction check
    ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    --> Finished Dependency Resolution

    Dependencies Resolved

    =============================================================================================================================================================================================================================================
     Package                                                                       Arch                                             Version                                                 Repository                                      Size
    =============================================================================================================================================================================================================================================
    Installing:
     python2-pip                                                                   noarch                                           8.1.2-10.el7                                            epel                                           1.7 M
    Installing for dependencies:
     python-backports                                                              x86_64                                           1.0-8.el7                                               base                                           5.8 k
     python-backports-ssl_match_hostname                                           noarch                                           3.5.0.1-1.el7                                           base                                            13 k
     python-ipaddress                                                              noarch                                           1.0.16-2.el7                                            base                                            34 k
     python-setuptools                                                             noarch                                           0.9.8-7.el7                                             base                                           397 k

    Transaction Summary
    =============================================================================================================================================================================================================================================
    Install  1 Package (+4 Dependent packages)

    Total download size: 2.1 M
    Installed size: 9.4 M
    Is this ok [y/d/N]: y
    Downloading packages:
    (1/5): python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch.rpm                                                                                                                                                   |  13 kB  00:00:00
    (2/5): python-backports-1.0-8.el7.x86_64.rpm                                                                                                                                                                          | 5.8 kB  00:00:00
    (3/5): python-setuptools-0.9.8-7.el7.noarch.rpm                                                                                                                                                                       | 397 kB  00:00:01
    (4/5): python-ipaddress-1.0.16-2.el7.noarch.rpm                                                                                                                                                                       |  34 kB  00:00:02
    warning: /var/cache/yum/x86_64/7/epel/packages/python2-pip-8.1.2-10.el7.noarch.rpm: Header V3 RSA/SHA256 Signature, key ID 352c64e5: NOKEY=========================================================-       ] 439 kB/s | 1.9 MB  00:00:00 ETA
    Public key for python2-pip-8.1.2-10.el7.noarch.rpm is not installed
    (5/5): python2-pip-8.1.2-10.el7.noarch.rpm                                                                                                                                                                            | 1.7 MB  00:00:03
    ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
    Total                                                                                                                                                                                                        547 kB/s | 2.1 MB  00:00:03
    Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    Importing GPG key 0x352C64E5:
     Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
     Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
     Package    : epel-release-7-11.noarch (@extras)
     From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    Is this ok [y/N]: y
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : python-backports-1.0-8.el7.x86_64                                                                                                                                                                                         1/5
      Installing : python-ipaddress-1.0.16-2.el7.noarch                                                                                                                                                                                      2/5
      Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch                                                                                                                                                                  3/5
      Installing : python-setuptools-0.9.8-7.el7.noarch                                                                                                                                                                                      4/5
      Installing : python2-pip-8.1.2-10.el7.noarch                                                                                                                                                                                           5/5
      Verifying  : python-ipaddress-1.0.16-2.el7.noarch                                                                                                                                                                                      1/5
      Verifying  : python-setuptools-0.9.8-7.el7.noarch                                                                                                                                                                                      2/5
      Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch                                                                                                                                                                  3/5
      Verifying  : python-backports-1.0-8.el7.x86_64                                                                                                                                                                                         4/5
      Verifying  : python2-pip-8.1.2-10.el7.noarch                                                                                                                                                                                           5/5

    Installed:
      python2-pip.noarch 0:8.1.2-10.el7

    Dependency Installed:
      python-backports.x86_64 0:1.0-8.el7                python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7                python-ipaddress.noarch 0:1.0.16-2.el7                python-setuptools.noarch 0:0.9.8-7.el7

    Complete!
# To install AWS CLI
       [vagrant@linux ~]$ sudo pip install awscli
        Collecting awscli
          Downloading https://files.pythonhosted.org/packages/8c/c1/61b505fce21669a0f7bf8973fe8a508e6537e4d5786d430bfd7ed023a9e1/awscli-1.16.262-py2.py3-none-any.whl (2.3MB)
            100% |████████████████████████████████| 2.4MB 242kB/s
        Collecting docutils<0.16,>=0.10 (from awscli)
          Downloading https://files.pythonhosted.org/packages/3a/dc/bf2b15d1fa15a6f7a9e77a61b74ecbbae7258558fcda8ffc9a6638a6b327/docutils-0.15.2-py2-none-any.whl (548kB)
            100% |████████████████████████████████| 552kB 534kB/s
        Collecting PyYAML<5.2,>=3.10; python_version != "2.6" and python_version != "3.3" (from awscli)
          Downloading https://files.pythonhosted.org/packages/e3/e8/b3212641ee2718d556df0f23f78de8303f068fe29cdaa7a91018849582fe/PyYAML-5.1.2.tar.gz (265kB)
            100% |████████████████████████████████| 266kB 759kB/s
        Collecting rsa<=3.5.0,>=3.1.2 (from awscli)
          Downloading https://files.pythonhosted.org/packages/e1/ae/baedc9cb175552e95f3395c43055a6a5e125ae4d48a1d7a924baca83e92e/rsa-3.4.2-py2.py3-none-any.whl (46kB)
            100% |████████████████████████████████| 51kB 792kB/s
        Collecting colorama<0.4.2,>=0.2.5; python_version != "2.6" and python_version != "3.3" (from awscli)
          Downloading https://files.pythonhosted.org/packages/4f/a6/728666f39bfff1719fc94c481890b2106837da9318031f71a8424b662e12/colorama-0.4.1-py2.py3-none-any.whl
        Collecting s3transfer<0.3.0,>=0.2.0 (from awscli)
          Downloading https://files.pythonhosted.org/packages/16/8a/1fc3dba0c4923c2a76e1ff0d52b305c44606da63f718d14d3231e21c51b0/s3transfer-0.2.1-py2.py3-none-any.whl (70kB)
            100% |████████████████████████████████| 71kB 730kB/s
        Collecting botocore==1.12.252 (from awscli)
          Downloading https://files.pythonhosted.org/packages/87/7d/58613fb1b75254770767f1e5e37f812ba27e9bac7d2bd8446dcae6f4d44e/botocore-1.12.252-py2.py3-none-any.whl (5.7MB)
            100% |████████████████████████████████| 5.8MB 76kB/s
        Collecting pyasn1>=0.1.3 (from rsa<=3.5.0,>=3.1.2->awscli)
          Downloading https://files.pythonhosted.org/packages/a1/71/8f0d444e3a74e5640a3d5d967c1c6b015da9c655f35b2d308a55d907a517/pyasn1-0.4.7-py2.py3-none-any.whl (76kB)
            100% |████████████████████████████████| 81kB 780kB/s
        Collecting futures<4.0.0,>=2.2.0; python_version == "2.6" or python_version == "2.7" (from s3transfer<0.3.0,>=0.2.0->awscli)
          Downloading https://files.pythonhosted.org/packages/d8/a6/f46ae3f1da0cd4361c344888f59ec2f5785e69c872e175a748ef6071cdb5/futures-3.3.0-py2-none-any.whl
        Collecting jmespath<1.0.0,>=0.7.1 (from botocore==1.12.252->awscli)
          Downloading https://files.pythonhosted.org/packages/83/94/7179c3832a6d45b266ddb2aac329e101367fbdb11f425f13771d27f225bb/jmespath-0.9.4-py2.py3-none-any.whl
        Collecting python-dateutil<3.0.0,>=2.1; python_version >= "2.7" (from botocore==1.12.252->awscli)
          Downloading https://files.pythonhosted.org/packages/41/17/c62faccbfbd163c7f57f3844689e3a78bae1f403648a6afb1d0866d87fbb/python_dateutil-2.8.0-py2.py3-none-any.whl (226kB)
            100% |████████████████████████████████| 235kB 543kB/s
        Collecting urllib3<1.26,>=1.20; python_version == "2.7" (from botocore==1.12.252->awscli)
          Downloading https://files.pythonhosted.org/packages/e0/da/55f51ea951e1b7c63a579c09dd7db825bb730ec1fe9c0180fc77bfb31448/urllib3-1.25.6-py2.py3-none-any.whl (125kB)
            100% |████████████████████████████████| 133kB 708kB/s
        Collecting six>=1.5 (from python-dateutil<3.0.0,>=2.1; python_version >= "2.7"->botocore==1.12.252->awscli)
          Downloading https://files.pythonhosted.org/packages/73/fb/00a976f728d0d1fecfe898238ce23f502a721c0ac0ecfedb80e0d88c64e9/six-1.12.0-py2.py3-none-any.whl
        Installing collected packages: docutils, PyYAML, pyasn1, rsa, colorama, futures, jmespath, six, python-dateutil, urllib3, botocore, s3transfer, awscli
          Running setup.py install for PyYAML ... done
        Successfully installed PyYAML-5.1.2 awscli-1.16.262 botocore-1.12.252 colorama-0.4.1 docutils-0.15.2 futures-3.3.0 jmespath-0.9.4 pyasn1-0.4.7 python-dateutil-2.8.0 rsa-3.4.2 s3transfer-0.2.1 six-1.12.0 urllib3-1.25.6
        You are using pip version 8.1.2, however version 19.3 is available.
        You should consider upgrading via the 'pip install --upgrade pip' command.
