
## How bypass it

#### Have some posibilites to do this. But for it, I had used the jump method.

```code
  address 0x7FF76F3315E5
```

| Address   | Kind       | Desc                           |
| :---------- | :--------- | :---------------------------------- |
| `0x7FF76F3315E5` | `conditional` | **conditional**. In this address you will found the main controlflow this binary |

#### Explain

How do you can bypass the main control flow, without have this? Get it. In logical programming, for check if a user is really a user, need a conditional. So found it.

You can use your favorite debugger for make this.
![image](https://github.com/iGutobreks/something/assets/68618064/31521a56-1ec7-4a57-889a-6dcb331109d1)
JZ basicly is mnomic check if zero, if thurth jump for the address.
If your input is incorrect, zero flag is equal one.
![image](https://github.com/iGutobreks/something/assets/68618064/0f5e7d46-dde0-498d-9faa-a7a85aaea775)

For bypass this, your task is just change the zero flag for zero.

This idea of zero flag in c:
```c
...
int cmp() {
  if (1 == 1) {
    return 0;
  }
  return 1;
}

int main(void) {
  cmp();
  retun EXIT_SUCCESS;
}
```
