# Artoolkit Barcode Markers collection

A collection of ready-to-use Barcode markers.

I created all markers for each kind of configuration.
You can see the following table for details.

Markers are on separate folders. Look out for folder name for marker configurations, and file names for the specific value of each barcode.

I generated only Barcode markers with an *Hamming Distance* greater than 0, otherwise they will be practically unusable.
Just remember: the higher the *Hamming distance*, the better for recognization.

**Important**
Keep in mind that when you add this spec on your AR.js scene: `...detectionMode: mono_and_matrix; matrixCodeType: 3x3;’` you are using the `AR_MATRIX_CODE_3x3` (so refer to the markers inside the "3x3" folder on this repo).

## Is there a live version of a barcode marker generator?

Yes, there is: [https://au.gmented.com/app/marker/marker.php](https://au.gmented.com/app/marker/marker.php)

But it is not open source and who knows for how long it will remain online. So for now it works. In case it stops working, you can still use the markers on this repo.

## Available markers

| Matrix code type                     | Folder name                 | Maximum number of markers  | Hamming distance |
| ------------------------------------ | --------------------------  | -------------------------- | ---------------- |
| AR\_MATRIX\_CODE\_3x3      |  3x3                           | 64                         |                 |
| AR\_MATRIX\_CODE\_3x3\_PARITY65      |  3x3_parity_6_5                           | 32                         | 1                |
| AR\_MATRIX\_CODE\_3x3\_HAMMING63     |  3x3_hamming_6_3                         | 8                          | 3                |
| AR\_MATRIX\_CODE\_4x4\_BCH\_13\_9\_3 |  4x4_bch_13_9_3              | 512                        | 3                |
| AR\_MATRIX\_CODE\_4x4\_BCH\_13\_5\_5 |  4x4_bch_13_5_5             | 32                         | 5                |
| AR\_MATRIX\_CODE\_5x5\_BCH\_22\_7\_7 |  5x5_bch_22_7_7              | 128                        | 7
| AR\_MATRIX\_CODE\_5x5\_BCH\_22\_12\_5 | 5x5_bch_22_12_5               | 4096                       | 5

# Learn more

* [Theory behind Barcode Markers](https://github.com/nicolocarpignoli/artoolkit-docs)

* [Artoolkit5](https://github.com/artoolkit/artoolkit5)

* [JSArtoolkit5 from ArtoolkitX project](https://github.com/artoolkitx/jsartoolkit5)

* [More informations about BCH and Hamming Distance relation - source code](https://gitlab.ida.liu.se/minnesmark/Minnesmark/blob/899a04de679477b59acbc0fbb114497229b9e05f/Minnesmark/ARToolKit/include/AR/ar.h)

# Credits

🐈 Thanks to [@fquffio](https://github.com/fquffio) for this.
