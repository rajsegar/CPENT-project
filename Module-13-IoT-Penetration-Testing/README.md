# Module 13: IoT Penetration Testing

## In plain language

Internet of Things (IoT) testing examines a complete connected-device system:
hardware, firmware, local interfaces, network services, companion applications,
cloud APIs, update mechanisms, and the device's physical and safety context.
The device is only one part of its attack surface.

## Key ideas

| Term | Beginner-friendly meaning |
| --- | --- |
| Firmware | Software stored on and executed by a device |
| Bootloader | Early code that starts the device and loads its operating software |
| Hardware interface | A physical debug or communication connection |
| Companion app | Mobile or desktop software used to manage a device |
| Update chain | How firmware is obtained, verified, installed, and rolled back |
| Device identity | Keys, certificates, or records that distinguish one device |
| Safety impact | Possible physical, environmental, or human consequence |
| Software bill of materials | An inventory of included software components |

## A safe assessment approach

1. Confirm device ownership, model, firmware version, region, and safety limits.
2. Diagram the device, local network, app, cloud service, users, and data flows.
3. Record every physical, wireless, network, software, and update interface.
4. Review vendor documentation and normal behavior.
5. Analyze a vendor-provided or lab firmware image in isolation.
6. Validate one approved hypothesis with minimal device change.
7. Restore or reflash the lab device and verify normal operation.

IoT findings can have consequences beyond confidentiality. A test plan should
consider bricking, battery damage, overheating, unsafe actuation, availability,
warranty, shared radio spectrum, and personal data.

## Common mistakes

- Testing the device while ignoring its cloud API and companion app.
- Assuming identical model names have identical hardware or firmware.
- Extracting keys and then committing them to notes.
- Flashing firmware without a known recovery method.
- Sending high-volume traffic to a resource-constrained device.
- Treating a component version as proof of reachable vulnerability.
- Ignoring safety and privacy consequences.

## Defender view

Useful defenses include unique device identities, secure boot, signed updates,
protected secrets, minimized services, safe recovery, encrypted communication,
server-side authorization, supported component inventories, vulnerability
disclosure, and lifecycle patch planning.

## Quiz

1. Why is an IoT device not the whole IoT attack surface?
2. What should be known before changing firmware?
3. Why is a component version alone incomplete vulnerability evidence?
4. Name three possible physical or availability risks of testing.
5. What is the purpose of a device-specific identity?

## Answer key

1. Apps, cloud APIs, local networks, update services, accounts, and physical
   interfaces also handle trust and data.
2. Exact model and version, authorization, trusted image, backup, recovery
   method, power requirements, and safety limits.
3. The component may be patched, configured differently, unreachable, or not
   used in the vulnerable way.
4. Examples include bricking, unsafe actuation, overheating, battery damage,
   radio interference, and service interruption.
5. It lets the system authenticate and authorize one device without relying on
   a universal shared secret.

## Flashcards

**Q:** What is firmware?  
**A:** Software stored on a device that controls its operation.

**Q:** What is secure boot?  
**A:** A process that verifies trusted software before allowing it to run.

**Q:** Why are shared device secrets risky?  
**A:** Compromise of one secret may affect many devices.

**Q:** What does an update chain protect?  
**A:** The authenticity and integrity of software delivered to a device.

**Q:** What is the first physical-device safety question?  
**A:** How the device can be restored if testing fails.

## Safe practical exercise

Use a course-provided IoT image, an intentionally vulnerable emulator, or a
spare device that you own and can recover. Do not connect it to a production or
public network.

Create a system diagram and interface inventory. Perform static review of an
approved firmware image and record its hash, file types, apparent components,
configuration clues, and possible secrets. Do not publish extracted secrets.
Choose one observation and describe the additional evidence needed before
calling it a vulnerability.

## Completion checklist

- [ ] I can map hardware, firmware, app, cloud, network, and update surfaces.
- [ ] I understand recovery and safety planning.
- [ ] I distinguish component identification from verified vulnerability.
- [ ] I completed static review in an isolated lab.
