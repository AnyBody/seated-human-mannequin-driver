# Seated human model with mannequin drivers for the limbs
This is a modified example of the [SeatedHuman](https://anyscript.org/ammr/Applications/Daily-activities-and-ergonomics/SeatedHuman.html) model in the AnyBody Managed Model Repository (AMMR). This example allows the limb postures to be set through the mannequin drivers.

There are switches in the Main file:
* REMOVE_LEGREST: When set to 1, the legrest is removed from the model. The footrest, which was originally attached to the legrest, is then driven with respect to the H point on the seat.
* USE_LEG_MANNEQUIN_DRIVERS: When set to 1, the leg posture can be driven through the Mannequin file in the Model folder. All the leg joint angles can be set except for hip flexion. Hip flexion is indirectly controlled by a constraint that ensures the heel point is in contact with the footrest.
* USE_ARM_MANNEQUIN_DRIVERS: When set to 1, the arm posture can be driven through the Mannequin file in the Model folder. You can drive all the joint angles of the arm.

This model was prepared for a client meeting for use-case in an automotive application.

## Usage
* Clone this repository.
* Update the libdef file to include a pointer to the libdef in your AMMR copy.
