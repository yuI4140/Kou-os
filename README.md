![Kou-os](Kou-os.png) 

![travis build](https://img.shields.io/badge/Version-1.0-%23ff1744)

a project to learn how to make an OS.

## Usage
- *Frist you need to install rust nighty*

   `` rustup default nightly ``

- *then just in case we add this component to rustup*

   `` rustup component add rust-src --toolchain nightly-x86_64-pc-windows-msvc ``
   
 > by the way, I think this is only on Windows if you have another OS you can avoid this part.


- *then you type*: 

` cargo install bootimage;cargo bootimage `

> remember cargo install bootimage is only for install 
>
> then you can do cargo bootimage where src/main.rs is update or not

- *a .bin file will be made in the debug folder of the project
 now you can boot it in a virtual machine or copy it to a USB drive to boot it on real hardware*


### Example

*we are using QEMU how a vertual machine*

``` qemu-system-x86_64 -drive format=raw,file=target\x86_64\debug\bootimage-kernrust-toolchainel.bin ```

#### output
![Example](ex.png)

## Links
[Writing an OS in Rust](https://os.phil-opp.com/)
## Status
Paused




