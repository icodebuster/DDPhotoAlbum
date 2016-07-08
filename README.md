DDPhotoAlbum
===================================
  iOS library that provides for multiple image selection.<br />
  
Installation
-----------------------------------
  Download DDPhotoAlbum and try out the included iPhone example apps<br />

Requirements
-----------------------------------
* iOS 7.0+<br />
* ARC<br />

Usage
-----------------------------------

### Manual import：
* Drag All files in the DDPhotoAlbum folder to project<br />
* Use by including the following import:<br>
    #import "DDPhotoAlbum.h"

### Open the Album
    DDPhotoAlbumViewController *photoAlbumViewController = [[DDPhotoAlbumViewController alloc]init];
    photoAlbumViewController.maxPhotos = 9;
    photoAlbumViewController.isShowCamera = YES;
    [photoAlbumViewController setDidSelectedBlock:^(NSArray *images, NSArray *thumbnailImages) {
        //handle photos
    }];
    [self presentViewController:photoAlbumViewController animated:YES completion:nil];

License
-----------------------------------
  AFNetworking is released under the MIT license. See LICENSE for details.<br />
