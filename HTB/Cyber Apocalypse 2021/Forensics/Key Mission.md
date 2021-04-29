# Key Mission

Looking at the packet capture we notice USB interrupt data. Whenever someone presses a key on a keyboard they cause an interrupt. So let's try keystroke mapping.
((usb.transfer_type == 0x01) && (frame.len == 72)) && !(usb.capdata == 00:00:00:00:00:00:00:00)

![image](https://user-images.githubusercontent.com/61699641/116568430-62589a00-a900-11eb-9def-041270436e57.png)

Above: filtering by only interrupt data.

Then export it to a csv and cut all columns except the HID one (key codes).

Then running [mapper.py](https://gist.githubusercontent.com/pdelteil/c033e0fa8cf2c80ad6b52ce867b30384/raw/96da8609c697838c168f2874d416670bccfb0c2a/mapper.py) with the hexcodes file gives: CHTB{a_plac3_fAr_fAr_away_fr0m_eaedelrth}
Adjusted for delete key: CHTB{a_plac3_fAr_fAr_away_fr0m_earth}

Note: Other scripts don't account for key buffering which is why I struggled at first as I didn't know what parts were capitalized due to shift being pressed.

Solved by Karim
