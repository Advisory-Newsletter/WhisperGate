# WhisperGate

**Indicators of Compromise**
1) SHA256 hash of The installer component for the bootloader -  a196c6b8ffcb97ffb276d04f354696e2391311db3841ae16c8c9f56f36a38e92

2) The destructive wiping operation has the following pseudocode:

for i_disk between 0 and total_detected_disk_count do
   for i_sector between 1 and total_disk_sector_count, i_sector += 199, do
      overwrite disk i_disk at sector i_sector with hardcoded data
   done
done

**References**
1) https://www.pcrisk.com/removal-guides/22801-whispergate-ransomware#quicksol
2) https://www.crowdstrike.com/blog/technical-analysis-of-whispergate-malware/
3) https://unit42.paloaltonetworks.com/ukraine-cyber-conflict-cve-2021-32648-whispergate/#hunting-for-whispergate
4) https://www.microsoft.com/security/blog/2022/01/15/destructive-malware-targeting-ukrainian-organizations/
