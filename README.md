set of empty folders for an 8-week college class, Each weeks folder has a "Screenshots" folder, and a "resources" folder, within. 





created by:
```
usern@MyLaptop:~$ mkdir CourseNum
usern@MyLaptop:~$ cd CourseNum/
usern@MyLaptop:~/CourseNum$ for i in $(seq 1 8); do     mkdir -p "Module $(printf '%02d' $i)"; done
usern@MyLaptop:~/CourseNum$ for i in {1..8}; do     mkdir -p "./Module 0$i";     mkdir -p "./Module 0$i/Screenshots";     mkdir -p "./Module 0$i/resources"; done
usern@MyLaptop:~/CourseNum$ tree
.
├── Module 01
│   ├── resources
│   └── Screenshots
├── Module 02
│   ├── resources
│   └── Screenshots
├── Module 03
│   ├── resources
│   └── Screenshots
├── Module 04
│   ├── resources
│   └── Screenshots
├── Module 05
│   ├── resources
│   └── Screenshots
├── Module 06
│   ├── resources
│   └── Screenshots
├── Module 07
│   ├── resources
│   └── Screenshots
└── Module 08
    ├── resources
    └── Screenshots

25 directories, 0 files
usern@MyLaptop:~/CourseNum$ 
```
