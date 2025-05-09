# cs2-fov-changer
cs2-fov-changer is a minimalistic C++ tool for changing Field of View (FOV) values in Counter-Strike 2 by directly accessing process memory. The program works at user-space level and uses Windows API to get process descriptor, fetch client.dll address, read and write FOV values by offset.
