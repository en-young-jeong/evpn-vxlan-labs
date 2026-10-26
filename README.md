# evpn-vxlan-labs

# EVPN VXLAN: L2 VNI vs. L3 VNI

## 1. L2 VNI
- Identifies a Layer 2 broadcast domain carried over VXLAN.
- Different VLANs commonly use different L2 VNIs.

## 2. L3 VNI
- Used to carry Layer 3 traffic associated with a VRF in EVPN VXLAN designs.
- Multiple L2 VNIs can be associated with the same VRF and L3 VNI.

## 3. Example

| VLAN | L2 VNI | VRF | L3 VNI |
|---|---:|---|---:|
| VLAN 10 | 10010 | BLUE | 50000 |
| VLAN 20 | 10020 | BLUE | 50000 |

## 4. Key takeaway
Different L2 segments can share a Layer 3 routing domain. L2 VNI and L3 VNI serve different purposes.
