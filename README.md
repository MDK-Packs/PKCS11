# PKCS11
This repo frames the OASIS PKCS 11 TC as a CMSIS-PACK (upstream: https://github.com/oasis-tcs/pkcs11)

# Instructions
1) open a bash compatible shell
2) clone repository: git clone https://github.com/MDK-Packs/PKCS11.git
3) run ./get_upstream.sh
4) run ./add_merge.sh to copy files from contributions/add to 'local' directory

a) Creating the CMSIS pack:
   1) run ./gen_pack.sh
   2) install the pack created in ./pack directory (e.g. double click on the pack file)

b) Making changes to the CMSIS pack:  
   You can develop and extend this pack further by contributing via GitHub:  
   https://github.com/MDK-Packs/PKCS11  
   All contributions shall be placed in either:  
   i)  contributions/add (additional content)  
   ii) contributions/merge (changed content)  
   To update your local pack content run ./add_merge.sh.  
   You can add the .../local/Arm-Packs.PKCS11.pdsc to the list of local repositories in the PackInstaller.  
   This way you avoid to create and install a new pack after modifications.

c) Alternatively you can contribute to the upstream repository  
   (see: https://github.com/oasis-tcs/pkcs11/blob/master/CONTRIBUTING.md)  
   run ./get_upstream.sh vX.Y.Z to download an updated upstream revision  
   add a new release tag and release description to the PDSC file (contributions/add/MDK-Packs.PKCS11.pdsc)  
   Note: please review all files in the 'merge' folder, as they may require updating to reflect changes
   of the upstream repository.

