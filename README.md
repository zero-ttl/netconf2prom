# ZeroNetconf
Prometheus Client populated by netconf retrieved data

-- config file


[default] # mandatory section

username = username # mandatory

password = password # mandatory

[actionbatch1]    # a single batch is supported

action = getBgpAdvPrefixes # mandatory

server_port = 8000 # mandatory

sleeping_period = 300 #mandatory (in s)

  [actionbatch1.router1]

    router = router1
    
    peers = ['149.14.132.245', '217.29.66.253' ]
    
    instance = inet.0

  [actionbatch1.router2]
    
    router = router2
    
    peers = ['80.249.208.100', '193.201.28.38' ]
    
    instance = inet.0


