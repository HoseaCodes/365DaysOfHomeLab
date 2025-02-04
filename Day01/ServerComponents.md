# Server Component Selection Guide

## 1. Processor (CPU)
### Key Considerations
- **Cores/Threads**: More cores allow for better virtualization
- **Clock Speed**: Higher speeds benefit single-threaded applications
- **TDP**: Power consumption and cooling requirements
- **Socket Type**: Determines motherboard compatibility

### Recommendations
#### Entry Level
- Intel Xeon E-2200 series
- AMD Ryzen 5/7 (Desktop grade but good for homelab)

#### Mid Range
- Intel Xeon Silver 4300 series
- AMD EPYC 7002 series

#### High End
- Intel Xeon Gold 6300 series
- AMD EPYC 7003 series

## 2. Motherboard
### Key Considerations
- **Form Factor**: ATX, E-ATX, SSI EEB
- **PCIe Slots**: For expansion cards
- **Memory Slots**: Number and type of supported RAM
- **IPMI**: Remote management capability
- **NIC**: Number and speed of network ports

### Recommendations
#### Entry Level
- Supermicro X11SCL-F
- ASRock Rack E3C246D4U

#### Mid Range
- Supermicro X12SPL-F
- ASUS WS C621E SAGE

## 3. Memory (RAM)
### Key Considerations
- **Type**: DDR4/DDR5, ECC vs non-ECC
- **Speed**: MHz rating
- **Capacity**: Total GB needed
- **Channels**: Dual/Quad channel support

### Recommendations
- Minimum: 32GB for basic virtualization
- Recommended: 64GB-128GB for multiple VMs
- Optimal: 256GB+ for extensive virtualization
- Brand suggestions: Samsung, Micron, Kingston

## 4. Storage
### System Drive
- **Type**: NVMe SSD recommended
- **Capacity**: 250GB-500GB minimum
- **Recommended**: Samsung 970 PRO, Intel DC series

### Data Storage
- **Type**: Mix of SSDs and HDDs
- **Configuration**: RAID options
- **Recommendations**:
  - SSDs: Samsung 860/870 PRO, Intel DC series
  - HDDs: WD Red Pro, Seagate IronWolf Pro

## 5. Power Supply (PSU)
### Key Considerations
- **Wattage**: Calculate total system power needs
- **Efficiency**: 80+ Gold minimum recommended
- **Redundancy**: Dual PSU option
- **Form Factor**: ATX vs Server PSU

### Recommendations
- Entry: Seasonic Focus Plus Gold 750W
- Mid: Corsair HX1000i
- High: Server grade redundant PSUs

## 6. Cooling
### Components
- **CPU Cooler**: Air vs Liquid
- **Case Fans**: Number and size
- **Airflow**: Front to back

### Recommendations
- **Air Cooling**: Noctua NH-U12S
- **Case Fans**: Noctua NF-A12x25 PWM
- **Fan Configuration**: Minimum 3 intake, 2 exhaust

## 7. Case
### Considerations
- **Form Factor**: Tower vs Rackmount
- **Drive Bays**: Number and type
- **Airflow**: Ventilation design
- **Cable Management**: Space and features

### Recommendations
#### Tower Cases
- Entry: Fractal Design Define 7
- Mid: Phanteks Enthoo Pro 2
- High: Corsair Obsidian 1000D

#### Rackmount Cases
- Entry: 4U Rosewill RSV-L4500U
- Mid: 2U Supermicro SC823
- High: 4U Supermicro SC846

## 8. Network Interface Cards (NICs)
### Considerations
- **Speed**: 1Gb vs 10Gb
- **Ports**: Number of connections
- **Type**: Copper vs Fiber

### Recommendations
- Entry: Intel I350-T4
- Mid: Mellanox ConnectX-3
- High: Intel X710

## Budget Planning
### Entry Level Build (~$1000-1500)
- CPU: Ryzen 7 5800X
- RAM: 32GB ECC
- Storage: 500GB NVMe + 2x4TB HDD
- Case: Tower format

### Mid Range Build (~$2500-3500)
- CPU: Xeon Silver 4310
- RAM: 128GB ECC
- Storage: 1TB NVMe + 4x8TB HDD
- Case: 4U Rackmount

### High End Build ($5000+)
- CPU: Dual Xeon Gold
- RAM: 256GB+ ECC
- Storage: 2TB NVMe + 8x12TB HDD
- Case: 4U Rackmount with redundant PSUs

## Additional Considerations
- **Noise Levels**: Important for home environment
- **Power Consumption**: Impact on electricity bills
- **Upgrade Path**: Future expansion possibilities
- **Warranty**: Especially for critical components
- **Used Enterprise Hardware**: Cost-effective alternative

## Component Testing Plan
1. Memory stress testing (Memtest86+)
2. CPU stress testing (Prime95)
3. Storage benchmark (CrystalDiskMark)
4. Network testing (iperf3)
5. Temperature monitoring under load
