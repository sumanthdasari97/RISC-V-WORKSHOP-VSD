# RISC-V-WORKSHOP-VSD
# OPENLANE DIRECTORY AND PDK DIECRTORY
![Screenshot from 2024-05-15 00-21-49](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/e1161ee2-5cc8-4398-b43e-aed0de3ba4cc)

![Screenshot from 2024-05-15 00-24-47](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/5e88de70-0575-4ca4-b9c9-18cf727ecd54)
# Invoking OpenLane 
![Screenshot from 2024-05-15 03-10-05](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/71796b9d-c6e2-4124-8f4a-1bce4f1e90f6)
# Installing Required Packages For Openlane
#command package require openlane 0.9
![Screenshot from 2024-05-15 03-11-18](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/1dd4f888-b089-4764-8ab2-bcb1eb57fd2e)
# Preapre and setup the design 
prep -design picorv32a
![Screenshot from 2024-05-15 03-17-58](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/b5811317-5e79-4a84-84ca-40bedc7edb8e)
setup happend in the design folder 
![Screenshot from 2024-05-15 03-19-10](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/040c75e6-5253-48d3-b230-f8d6b7b760e7)
# **Synthesis**
#command run_synthesis
![Screenshot from 2024-05-15 04-14-54](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/4d435aa9-f8f3-4789-8d68-60c9471cac53)
_Sythesis Reports_
# Flop Ratio = 1613/14876 = 10.8%
![Screenshot from 2024-05-15 04-20-49](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/20deeb0f-c876-49a0-8dff-5645e5aca827)
Chip_Area for module =147712.918400
![Screenshot from 2024-05-15 04-26-15](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/ada3f937-9613-4633-a57e-6d96877c02ad)
Successful_synthesis
![Screenshot from 2024-05-15 04-31-37](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/17c2cdf2-0c8d-44cb-9a08-75cdcf248fe1)
synthesized_netlist  in Results
![Screenshot from 2024-05-15 04-37-05](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/1e97ee11-5482-4e47-8231-bf94c243c3ef)
Configuration tcl file for picorv32a design
![Screenshot from 2024-05-15 05-23-27](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/f11aa0b7-5278-48e7-be24-716fb6bb6f0c)

# **Running floor Plan**
  %run_floorplan
![Screenshot from 2024-05-15 05-32-22](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/5fd886ea-fb83-43e7-806e-d2ae84b1e372)
Insertion of Physical Cells
![Screenshot from 2024-05-15 05-38-11](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/59b9a186-2d85-408f-8a99-a4ff26f6ca69)

Floor_Plan.def 
![Screenshot from 2024-05-15 05-45-52](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/e7bd571e-99b9-426e-96ef-f3ecceb1111a)

# Layout in magic
to invoke magic gui 
/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/14-05_21-43/results/floorplan$ magic -T /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def &

![Screenshot from 2024-05-15 06-30-01](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/4d042df5-30bd-4885-bfc4-ff275d66abed)

Selected Cell description from console by giving command what
![Screenshot from 2024-05-15 07-05-05](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/4670ecb6-855d-4dd1-859a-2a116a5e5282)

# Placement
%run_placement 
![Screenshot from 2024-05-15 07-26-14](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/2c412b8e-be94-4329-ad6c-bc27718a53c7)

placement in magic gui 
![Screenshot from 2024-05-15 07-29-54](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/4bdb2758-e911-4712-9705-a9ffa7d3f50f)

zoomed pic of placement of standard cells
![Screenshot from 2024-05-15 07-31-12](https://github.com/sumanthdasari97/RISC-V-WORKSHOP-VSD/assets/161044842/21ee9c48-c5c1-4bce-9154-2065a1959de0)













