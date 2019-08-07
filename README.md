# Coding Syntax Memo

## Summary

## Content

声明一个 block 和 block 属性


`Objective-C`

```objc
typedef void (^DidSelectHandler)(NSInteger index);

@property (nonatomic, copy) DidSelectHandler didSelectHandler;
```


声明一个 protocol 和 delegate 属性

`Objective-C`

```objc
@protocol RatioSelectViewDelegate <NSObject>
- (void)didSelectRowAt:(NSInteger) index;
- (void)didCancel;
@end

@property (weak, nonatomic) id <RatioSelectViewDelegate> delegate;

```