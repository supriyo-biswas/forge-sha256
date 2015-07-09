Reason to use this instead of the official forge build:
  - drastic size reduction by pruning all unecessary code for SHA-256 , from 284K to 4.5K
  - automatically sets right encoding
  
Targets the browser.

Code extracted from [forge's master on July 2015](https://github.com/digitalbazaar/forge/tree/3b7826f7c2735c42b41b7ceaaadaad570e92d898).

#### Usage
```
<script src='build/forge-sha256.min.js'></script>
<script>
console.log(forge_sha256('abc'));
// prints ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad
</script>
```
`forge_sha256()` handles both ASCII and UTF-8 strings.