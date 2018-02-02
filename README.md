# ArcLine

VRML PROTO (based on `IndexedLineSet`) that generates the outline for part of a flat circle (e.g. for **pie charts**),
similar to [PROTO Arc](https://github.com/wildpeaks/proto-arc).

	EXTERNPROTO ArcLine [
		exposedField  SFFloat  fromAngle
		exposedField  SFFloat  toAngle
		exposedField  SFFloat  radius
		exposedField  SFFloat  tesselation
		exposedField  SFBool   beginCap
		exposedField  SFBool   endCap
	] "proto.ArcLine.wrl#ArcLine"


-------------------------------------------------------------------------------

## Property `fromAngle`

**Start angle** (in radians).

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `0`


-------------------------------------------------------------------------------

## Property `toAngle`

**End angle** (in radians).
If `toAngle > fromAngle`, the mesh is generated **clockwise**, otherwise **anti-clockwise**.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `6.28318`


-------------------------------------------------------------------------------

## Property `radius`

**Radius** of the circle.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `1`


-------------------------------------------------------------------------------

## Property `tesselation`

Intermediary steps on the curve.
In short, **higher tesselation = rounder shape = more vertices**.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `16`


-------------------------------------------------------------------------------

## Property `beginCap`

When `TRUE`, it adds a line segment from the center of the circle to the beginning of the curve.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFBool`
 - Default Value: `TRUE`


-------------------------------------------------------------------------------

## Property `endCap`

When `TRUE`, it adds a line segment from the center of the circle to the end of the curve.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFBool`
 - Default Value: `TRUE`


-------------------------------------------------------------------------------

