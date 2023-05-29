~~~~
----------------------------------------------------------------------
 Hellminer 0.59.1 [VerusHash 2.2 + PBaaS] Linux
----------------------------------------------------------------------
Usage: hellminer [options]

Options:
  -h, --help            show this help message and exit
  -l, --list            Show CPU information and exit
  -c URL, -o URL, --pool=URL
                        stratum+ssl://WALLET.RIG:pass@host:port
                        stratum+tcp://WALLET.RIG@host:port
                        stratum+tcp://WALLET@host:port
  -u WALLET.RIG, --user=WALLET.RIG, --wallet=WALLET.RIG
                        Specify wallet address; overridden if in URL
  -p x, --pwd=x, --pass=x, --password=x
                        Password parameters for pool; overridden if in URL
  --dual-pool=URL       Split hashing between two pools:
                        stratum+ssl://pool.verus.io:19999 * Note, this only
                        works good on systems capable of at least 5+ MH/s
  --dual-pass=URL       If needed, specify a different password for the dual
                        pool.
  --cpu=N, --threads=N  Use N threads on CPU (default: 1, max_threads: 254)
  --priority=N          priority; 1=normal,2=lower (default: 1)
  --numa=N              experimental numa node selection support: 1, 2, 3, 4
  --affinity            experimental auto thread affinity
  --ssl, --tls          Force using SSL connection
  --keep-alive          Send 'keepalived' stratum method to pool for
                        stimulating data flow after 30 seconds of no data
                        flow. *Note special feature not all pools support
  --ping                Send 'mining.ping' stratum method to pool for
                        stimulating data flow after 30 seconds of no data
                        flow. *Note special feature not all pools support
  --api-port=8080       http://localhost:8080/ [0 = default, 8080 = enable]
  --api-pass=PASS       Enable '/admin' API access in browser using password
  --no-colors           Disable console colors
  -v, --verbose         Output more debug information
~~~~
### Requirements
A procesor with SSE4 and/or AVX, AVX2 intrinsic instruction set.  
If your processor does not support AVX, do not download the AVX version (it will fail)
  > Windows: Requires Visual C++ 2022 Runtime [vc_redist.x64](https://aka.ms/vs/17/release/vc_redist.x64.exe)
  
  > Linux  : May need `sudo apt install libsodium-dev`
  >
### [Download](https://github.com/hellcatz/hminer/releases)


### Known Hashrates:
  Intel i9-7900X (18 threads): 20.00MH/s  
  Intel i7-8700K (10 threads): 12.50MH/s  
  Intel i7-6700K (6 threads): 6.50MH/s  
  Intel i7-4790K (7 threads): 7.70MH/s  
  Intel i7-4170HQ (5 threads): 4.60MH/s  
  Intel i7-5500U (3 threads): 2.45MH/s  
  Intel i5-8600K (6 threads): 10.45MH/s  
  Intel i5-5200U (2 threads): 1.50MH/s    
  Intel i3-8100 (4 threads): 5.00MH/s  
  Intel i3-7100 (3 threads): 3.50MH/s  
    
  Dual Xeon E5-2697v2 (46 threads): 27.77MH/s  
  Dual Xeon E5-2620v2 (20 threads): 10.50MH/s  
  
  AMD ThreadRipper 3990X (4.1GHz OC) (128 threads): 168.00MH/s  
  AMD ThreadRipper 2990WX (63 threads): 72.00MH/s  
  AMD ThreadRipper 2970WX (47 threads): 62.00MH/s  
  
  AMD Opteron 6276 (31 threads): 15.62 MH/s  
  
  AMD Ryzen 3970X (49 threads): 57.00MH/s  
  AMD Ryzen 3950X (32 threads): 41.00MH/s  
  AMD Ryzen 3900X (24 threads): 31.10MH/s  
  AMD Ryzen 3800X (?? threads): 22.00MH/s  
  AMD Ryzen 2700X (14 threads): 16.00MH/s  
  AMD Ryzen 2700 (15 threads): 16.00MH/s  
  AMD Ryzen 1600 (10 threads): 11.00MH/s  
    
  AMD A10 (4 threads): 3.50MH/s  
