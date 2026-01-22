
#### **Permissions in linux are assigned on basis of** 

### User 

### Group 

### Other

#### Which is , u , g , o 

> In permissions we have 3 permissions , **Read**  , **Write** , **Exicute**

---

### Read = 4

### Write = 2 

### Execute = 1

### read + write + execute = 7
### 4        +    2      +     1         =  7



---
### How to identify user or group

### User , Group , Other 
### - - - , - - - , - - - 

### RWX , RWX , RWX            (Symbolic Notation)

### 421 , 421 , 421           ( Octal notation)

---
### Examples for understanding

1. if you want to give only read permission to the group 
```
chmod g+r file.txt

		OR
		
chmod 040 file.txt  
```


2. If you want to give execution permission to user and read to all others.

```
chmod u+r , go+r file.txt

        OR
		
chmod 744 file.txt
```

3. If you want to give executable permission to everyone.

```
chmod ugo+rwx file.txt 

		OR

chmod 777 file.txt
```


4. If you want to give 0 permission to user and all permission to others.

```
chmod u= , go=rwe file.txt

			OR

chmod 077 file.txt 
```

---


### Important Note on Ownership

**While you can set the owner's permissions to zero, as the owner of the file, you still retain the right to change its permissions back at any time using `chmod`. If you try to read or write the file while permissions are `0`, the system will deny you access until you change them again.**

---
