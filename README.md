# Defimist Solidity smart-contract flattened source file generation

### Installation from npm

`npm i defimist-solidity-flattener`

### Usage

`./node_modules/.bin/poa-solidity-flattener ./contracts/example.sol`

It will save flattened source of Solidity smart-contract into `./out` directory

### Installation from source


```
git clone https://github.com/defimist/defimist-solidity-flattener
cd defimist-solidity-flattener
npm install
```

You can start script either

```
npm start "path_to_not_flat_contract_definition_file.sol"
```

or without paramaters (path to input file will be extracted from `./config.json`)

```
npm start
```



Expected result: 

```
Success! Flat file ORIGINAL_FILE_NAME_flat.sol is generated to ./out directory
```

`./flatContract.sol` - flat .sol file is created in output directory (`./out/` by default)

**Note:** *utility doesn't support aliases at import statements*

## Config

path `./config.json`

```
{
	"inputFilePath": "./demo/src/Oracles.sol",
	"outputDir": "./out"
}
```

