# Etat futur
- idle+ = idle./ready + throw + moveInit.Done
- scan+ = idle.ready + scan.color1.color2
- throw+ = scan./color1./color2
- moveBlue+ = scan.color1./color2 + moveBlue./done
- moveRed+ = scan./color1.color2 + moveRed./done
- drop+ = moveBlue.done + moveRed.done
- moveInit+ = drop + moveInit./done