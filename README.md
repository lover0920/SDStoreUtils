# SDStoreUtils
类方法实现plist文件的存储和读取，归档和解归档，钥匙串的存储、读取、删除

```
#import <Foundation/Foundation.h>

@interface SDStoreUtils : NSObject
//plist文件的存储和读取
+ (void)saveArrayDataForPlistFile:(NSMutableArray *_Nullable)array
fileName:(NSString *_Nullable)fileName;
+ (NSArray *)readArrayDataFromePlistFile:(NSString *_Nullable)fileName;


//归档和解归档
+ (void)saveKeyedArchiverFile:(nullable id)responseObject
key:(NSString *_Nullable)key;
+ (nullable id)readKeyedUnarchiverFile:(NSString *_Nullable)key;
+ (void)deleteKeyedArchiverFile:(NSString *_Nullable)key;

//🔑钥匙串的存储、读取、删除
+ (void)saveKeychainValue:(NSString *_Nullable)sValue
key:(NSString *_Nullable)sKey;
+ (NSString *)readKeychainValue:(NSString *_Nullable)sKey;
+ (void)deleteKeychainValue:(NSString *_Nullable)sKey;
@end

```
