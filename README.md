# neovim_test

This container is based on Arch Linux and runs tests using [plenary.nvim](https://github.com/nvim-lua/plenary.nvim)

## Example of directory structure
<pre>        
├── docker-compose.yml     
├── Dockerfile  
├── README.md
└── tests
    ├── minimal.vim      
    ├── plugin1_spec.lua                                
    ├── plugin2_spec.lua                                
    └── plugin3_spec.lua                               
</pre>

## Usage

Each time you modify `Dockerfile` or `docker-compose.yml` run
```bash
docker-compose up --build
```

to run the tests
```bash
docker-compose run <service name>
```
