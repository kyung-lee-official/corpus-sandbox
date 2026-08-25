# Repair

New modelers often make several common mistakes, including inverted normals (flipped faces), non-manifold edges, un-merged vertices, etc. As these issues can lead to printing failures, CHITUBOX offers repair tools to resolve them.

## Error Detection

Error detection will help you locate issues like excess shell (pieces that are not connected to the main model, floating geometries, etc.), holes that making the model non-manifold, inverted normals.

Different error counts are displayed in the Parameters Panel.

Shells are typically imperceptible, they are listed in an individual list and can be highlighted for easier identification.

After fixing errors, you may need to re-detect to see if any issues remain.

## Model Repair

### Basic Repair

Basic Repair performs a series of automatic checks and fixes, trying to make your model manifold and ready for printing.

### Close Trivial Holes

Click **Close Trivial Holes** to automatically fix defected holes with 6 edges or less and missing surfaces. The program will fill these areas to ensure complete model surfaces for printing.

### Close All Holes

Click **Close All Holes** to automatically fix all damaged holes and missing surfaces in the model. The program will fill these areas to ensure complete model surfaces for printing.

### Orientation Repair

**Orientation Repair** will try to fix the orientation of your model's faces, making all normals face outward, which is crucial for successful printing.

### Coat Outer Surface

**Coat Outer Surface** will try to traverse the outer surface of your model, regenerating the surface, removing broken structures inside, ensuring it is manifold and suitable for printing.

## Triangle Repair

Triangle Repair tools can help you fix issues related to the triangular mesh of your model manually, such as non-manifold edges and flipped normals.

## Advanced Repair

Advanced repair will detect if your model is solid or not, and will try to remove any chamber inside the model.
