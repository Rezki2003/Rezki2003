import { Seaport } from "@opensea/seaport-js";
import { ethers } from "ethers";

// Provider must be provided to the signer when supplying a custom signer
const provider = new ethers.providers.JsonRpcProvider(
  "https://<network>.alchemyapi.io/v2/YOUR-API-KEY"
);

const signer = new ethers.Wallet("YOUR_PK", provider);

const seaport = new Seaport(signer);
