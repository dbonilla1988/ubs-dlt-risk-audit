'forge config --json' running
'/Users/davidbonillajaylen2022/.solc-select/artifacts/solc-0.8.27/solc-0.8.27 --version' running
'/Users/davidbonillajaylen2022/.solc-select/artifacts/solc-0.8.27/solc-0.8.27 @openzeppelin/contracts/=contracts/ contracts/token/ERC20/ERC20.sol --combined-json abi,ast,bin,bin-runtime,srcmap,srcmap-runtime,userdoc,devdoc,hashes --optimize --optimize-runs 200 --evm-version prague --allow-paths .,/Users/davidbonillajaylen2022/openzeppelin-contracts/contracts/token/ERC20' running
INFO:Printers:
Compiled with solc
Total number of contracts in source files: 7
Source lines of code (SLOC) in source files: 178
Number of  assembly lines: 0
Number of optimization issues: 0
Number of informational issues: 1
Number of low issues: 0
Number of medium issues: 0
Number of high issues: 0

ERCs: ERC20

+----------------+-------------+-------+--------------------+--------------+----------+
| Name           | # functions | ERCS  | ERC20 info         | Complex code | Features |
+----------------+-------------+-------+--------------------+--------------+----------+
| IERC721Errors  | 0           |       |                    | No           |          |
| IERC1155Errors | 0           |       |                    | No           |          |
| ERC20          | 29          | ERC20 | No Minting         | No           |          |
|                |             |       | Approve Race Cond. |              |          |
|                |             |       |                    |              |          |
+----------------+-------------+-------+--------------------+--------------+----------+
INFO:Slither:contracts/token/ERC20/ERC20.sol analyzed (7 contracts)
