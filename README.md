# Full Node Deployment via Monk.io 

## Requirements

1. Install Docker
2. Install Monk using this guide: https://docs.monk.io/docs/monk-in-10

## Mainnet setup: 

### From the CLI

1. 
    ```Monk load polygon-mainnet.yml```

2.
    ```Monk run polygon/heimdall-node```

3. 
    Check if heimdall is fully synced: 
        `curl http://localhost:26657/status`

4.
    ```Monk run polygon/bor-node```

## Testnet setup: 

1. 
    ```Monk load polygon-testnet.yml```

2.
    ```Monk run polygon/heimdall-node```

3. 
    Check if heimdall is fully synced: 
        `curl http://localhost:26657/status`

4.
    ```Monk run polygon/bor-node```


## One-command-setup:

1. 
    ```Monk load polygon-one-command.yml```

2. 
    ```Monk run polygon/node```


## Set up Prometheus and Grafana

1. 
    ```Monk load polygon-monitoring.yml```

2. 
    ```Monk run polygon/monitoring```

3. 
    Import json files in dashboards folder to grafana dashboard