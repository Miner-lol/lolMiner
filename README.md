# lolMiner 
### AMD & Nvidia & Intel Miner for Etchash, Autolykos2, Beam, Grin, Ae, ALPH, Flux, Equihash, Kaspa, Nexa, Ironfish, Conflux, Karlsen and Pyrin and more
### Best Dual Miner for ALPH and GRAM and KARLSEN and PYRIN and RADIANT with full Unlock LHR in all ALGOs

A git repository for lolMiner release versions

* Downloads releases : https://github.com/Lolliedieb/lolMiner-releases/releases
* Helpful information in : https://github.com/Lolliedieb/lolMiner-releases/wiki
* Telegram Group : https://t.me/lolMiner
* Discord Group :  https://discord.gg/jvfRvK5wTv
* Youtube Channel : https://www.youtube.com/c/lolMinerSupport

## Supported Algorithm

| Algorithm  | Fee % |
| ------------- | ------------- |
| Alephium | 0.75  |
| Autolykos V2 | 1.5  | 
| BeamHash III | 1.0  |
| Cuckoo 29 | 2.0  |
| CuckarooD 29 | 2.0 |
| CuckarooM 29 | 2.0 | 
| Cuckaroo 30 CTXC | 2.5 |
| Cuckatoo 31 | 2.0 |
| Cuckatoo 32 | 2.0 |
| Cuckaroo 29-32 | 1.0 |
| Cuckaroo 29-40 | 1.0 |
| Dual ETC + (KAS/ALEPH) | 1.0 / 0.0 |
| Dual ETH (ETHW) + (KAS/ALEPH) | 1.0 / 0.0 |
| Dual RTH + (ALEPH/GRAM//PYI/RXD) | 1.0 / 0.75 - 1.0 |
| Dual IRON + (ALEPH/GRAM/PYI/RXD) | 1.0 / 0.75 - 1.0 |
| Equihash 144/5 | 1.0 |     
| Equihash 192/7 | 1.0 |
| Equihash 210/9 | 1.0 |
| Etchash | 0.7 |
| Ethash (ETHW) | 0.7 |
| Ironfish | 1.00 |
| Kaspa | 0.75 |
| Karlsen | 1.0 |
| KarlsenV2 | 1.0 |
| Nexa | 2.0 |
| Octopus | 2.0 |
| Pyrin | 1.0 |
| PyrinV2 | 1.0 |
| Radiant | 0.75 |
| Rethereum | 1.00 |
| TON/GRAM | 1.00 |
| ZelHash (Flux) | 1.0 / 1.5 |


## Options supported by lolMiner
To see some basic configuration examples, see here: https://github.com/Lolliedieb/lolMiner-releases/wiki/lolMiner-Basic-usage-(English)

### General Options

Parameter | Description
| ------------- | ------------- |
|  -h [ --help ]                     |    Help screen |
|  --config arg (=./lolMiner.cfg)    |    Config file |
|  --json arg (=./user_config.json)  |    Config file in Json format |
|  --profile arg                     |    Profile to load from Json file |
|  --nocolor [=arg(=on)] (=off)      |    Disable colors in output |
|  --basecolor [=arg(=on)] (=off)    |    Use 16 colors scheme for non-rgb terminals |
|  --list-coins                      |    List all supported coin profiles |
|  --list-algos                      |    List all supported algorithms |
|  --list-devices                    |    List all supported & detected GPUs in your system |
|  -v [ --version ]                  |    Print lolMiner version number |

### Mining Options
| Parameter | Description |
| ------------- | ------------- |
|  -a [ --algo ] arg           |          The algorithm to mine.  |
|  -p [ --pool ] arg           |          Mining pool to mine on <br/> Format: <pool>:<port> |
|  -u [ --user ] arg           |          Wallet or pool user account to mine on |
|  --pass arg                  |          Pool user account password (Optional) |
|  --tls arg                   |          Toggle TLS ("on" / "off") |
|  --dns-over-https arg (=1)   |          Toggle dns over https. <br />0=default dns only <br />1=DoH with default dns as backup (default) <br />2=DNS over https enforced |
|  --devices arg                |         The devices to mine on <br /> Values: ALL / AMD / NVIDIA or a comma separated list of incidences.|
|  --devicesbypcie [=arg(=on)] (=off) |   Interpret --devices as list of PCIE BUS:SLOT pair|
|  --pers arg                   |         The personalization string. Required when using --algo for Equihash algorithms|
|  --keepfree arg (=5)          |         Set the number of MBytes of GPU memory that should be left free by the miner.|
|  --benchmark arg              |         The algorithm to benchmark|
|  --socks5 proxyPool:proxyPort |  For Socks5 connection  |
|  -c [ --coin ] arg           |          The coin to mine - this is an alternative to --algo that sets both, the algorithm and the personalization string for Equihash coins. (old)|
|  --max-latency     |   From v1.53 If the pool share latency is above this value and failover pools are configured, the miner will terminate the connection and connect to the next failover pool (at the earliest after 10 shares on the active connection). This is repeated if necessary until a pool remains below the latency limit. The default value is 0, which disables the feature. In dual-mining, multiple values can be specified separated by a comma, where the first value is for the first algorithm and the second is for the second algorithm. If only one value is specified, it applies to all connections. |

### Statistics Options:
Parameter | Description
| ------------- | ------------- |
|  --apiport arg (=0)                |    The port the API will use |
|  --apihost arg (=0.0.0.0)          |    The host binding the API will use |
|  --longstats arg (=60)             |    Long statistics interval |
|  --shortstats arg (=15)            |    Short statistics interval |
|  --statsformat arg (=default)       |   Format for long statistics. Use --help-format to get an overview of available fields. |
|  --hstats [=arg(=0)] (=-1)         |    Select stats to be drawn in a horizontal manner for each GPU. The number overwrites the terminal width detection. |
|  --vstats [=arg(=0)] (=0)          |   Select stats to be drawn in a vertical  manner for each GPU (default). The number overwrites the terminal width detection. |
|  --help-format [=arg(=1)]           |   Format description for --statsformat |
|  --digits arg                       |   Number of digits in hash speed after delimiter |
| --timeprint [=arg(=on)] (=off)      |  Enables time stamp on short statistics ("on" / "off") |
| --compactaccept [=arg(=on)] (=off)  |  Enables compact accept notification |
|  --log [=arg(=on)]                  |   Enables printing a log file ("on" / "off") |
|  --logfile arg                      |   Path to a custom log file location |

### Ethash Specific Options:
Parameter | Description
| ------------- | ------------- |
|  --ethstratum arg (=ETHPROXY)  |        Ethash stratum mode. Available options: ETHV1: EthereumStratum/1.0.0 (Nicehash) ETHPROXY: Ethereum Proxy |
|  --worker arg (=eth1.0)        |        Separate worker name for Ethereum Proxy stratum mode. |
|  --mode arg (=b)              |         Kernel mode to mine on. Comma separated values for configuring multiple cards differently. Use --mode a (faster) --mode b (better energy efficiency). In mixed system select 'a' for skipping over the AMD cards.  --mode s Added a split DAG mode for Nvidia GPUs in case that the memory allocation fails on the primary kernels. This will be a bit slower, but improve compatibility, especially for 5G GPUs. Use --mode s to force it.|
|  --lhrv3boost    | From v1.50 experimental LHR v3 unlock to ~90% (3050) and ~92% (3080 12G) (default enables) Use --lhrv3boost 0 to disable the mode and fall back to ~65% unlock. The experimental mode for LHR V3 seems to sometimes have unstable when starting up with only a reboot solving it - but after a first successful start it is stable - therefore the option to turn it off if you are struggling to start it up too many times. -When configuring the --lhrv3boost via json file, use "LHRV3BOOST" : 1 to set it. | 
|  --lhrtune arg (=auto)         |        Offset to most important LHR parameters. If your card is unstable or does not unlock try negative values. Range is +/-40. (old) |
|  --lhrwait arg (=0)            |        Time in seconds to wait after startup before any LHR detection or calibration takes place. (old) |
| --disable-dag-verify [=arg(=1)] (=0) |  Disable the CPU side verification and repair of DAG. |
|  --dagdelay [=arg(=0)] (=-1)     |      Delay between creating the DAG buffers for the GPUs. Negative values enable parallel generation (default). |
|  --enablezilcache [=arg(=1)] (=0) |     Allows 8G+ GPUs to store the DAG for mining Zilliqa. It will generated only once and offers a faster switching. |
|  --benchepoch arg (=440)       |        The DAG epoch the denchmark mode will use |

### Algorithm Split Options & Dual Mining Options:
Parameter | Description
| ------------- | ------------- |
|  --dualmode arg (=none)    |            Dual mode used. Allowed options: none, zil, zilEx, eth, etc, D-SPLIT, KASPADUAL, ALEPHDUAL,... |
|  --dualpool arg             |           Pool configuration for extra connection, Format <pool>:<port> |
|  --dualuser arg             |           Username or wallet address for the extra connection |
|  --dualpass arg              |          Password for the extra connection (Optional) |
|  --dualworker arg (=eth1.0)  |          Separate worker name for the 2nd connection. |
|  --dualtls arg               |          Toggle TLS ("on" / "off") for the 2nd connection. |
|  --dualdevices arg          |           Split rule for etc and beam split mode. Use a comma separated list of indexes or "4G" (default). |
|  --dualfactor arg          |           Solver will be dualfactor * Eth/Etc hash rate. So for example if the factor is 25 and the Eth hash rate is 59.5 mh/s, then the dual hash rate will be 25 times 59.5 mh/s = 1487,5 mh/s. The maximum dual factor at the moment is 64, a value of 0 will disable dual mining on the GPU |

### Managing Options:
Parameter | Description
| ------------- | ------------- |
|  --watchdog arg (=script)     |         Specify which action to take when a card is detected to be crashed. <br /> "off": Continue working on remaining cards. No action.  <br />"exit": Exit the miner with exit code 42 to ask for a restart. Recommended for Nvidia cards. <br /> "script": Call an external script. Default and recommended for AMD cards.  |
|  --watchdogscript arg      |            Specify which script to be executed when a hung GPU is detected |
|  --singlethread [=arg(=-1)] (=-2) |     Enable single mining thread mode for all GPUs (-1) or for a specific GPU id. |
|  --tstart arg (=0)           |          Minimal temperature for a GPU to start in degree C. If set to 0 disables restart below a fixed temperature. |
|  --tstop arg (=0)            |          Temperature to pause or stop a GPU from mining in degree C. If set to 0 disables stop above a fixed temperature. |
|  --tmode arg (=edge)         |          Mode for temperature management. Use "edge" (default), "junction" or "memory" to set the mode for temperature management. |
|  --ergo-prebuild arg (=-1)     |        Disable (0) or Enable (1) the function of pre-building the dataset for Ergo. -1 refers to the card default. |

### Overclock Options:
Parameter | Description
| ------------- | ------------- |
|  --cclk arg (=*)  | The core clock used for the GPUs. Cards are separated with a comma. "*" can be used to skip a card. |
|  --coff arg (=*)  | The core offset used for the GPUs. Cards are separated with a comma. "*" can be used to skip a card. |
|  --mclk arg (=*)  | The memory clock only used for KASPA/ALPH to reduce Watts with value 810. "*" can be used to skip a card. |
|  --moff arg (=*)  | The memory offset used for the GPUs. Cards are separated with a comma. "*" can be used to skip a card. |
|  --pl arg (=*)  | The power limit used for the GPUs. Cards are separated with a comma. "*" can be used to skip a card. |
|  --fan arg (=*)  | The % of the fan used for the GPUs. Cards are separated with a comma. "*" can be used to skip a card. |
|  --no-oc-reset  |  To avoid reset the overclock settings applied when ending the miner |



| GPU        | Range       | 
| ------------- |:-------------:| 
| 2070 | 1000 - 1050 |
| 2080 | 1110 - 1160 |
| 3060 (1) | 1070 - 1120 |
| 3060ti | 1300 - 1350 |
| 3070 | 750 - 800 |
| 3080 | 1010 - 1060 |


