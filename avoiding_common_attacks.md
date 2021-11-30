1.	SolarPanelNFT.sol will use Specific Compiler Pragma 0.8.0 (SWC-103 Floating Pragma => Contracts should be deployed with the same compiler version and flags that they have been tested with thoroughly. Locking the pragma helps to ensure that contracts do not accidentally get deployed using, for example, an outdated compiler version that might introduce bugs that affect the contract system negatively.)
2.	SolarPanelNFT.sol will protect against Modifiers making External Calls and Will Only for Be Used for Validations (SWC 107 Reentracy => Avoid external calls to avoid introducing malicious actors to the Smart Contract’s internal functionality)
3.	SolarPanelNFT.sol will use Check-Effects-Interactions to avoid state changes after external calls (SWC 107 Reentracy => Avoid external calls to avoid introducing malicious actors to the Smart Contract’s internal functionality)