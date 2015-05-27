# JHBlockActionSheet
支持block回调

使用方法
导入 #import "JHBlockActionSheet.h"

使用JHBlockActionSheetItem创建item
    JHBlockActionSheetItem *item1 = [JHBlockActionSheetItem itemWithTitle:@"1" andBlock:^{
        NSLog(@"1");
    }];

初始化ActionSheet
    JHBlcokActionSheet *action = [[JHBlcokActionSheet alloc] initActionSheetWithTitle:@"哈哈"
                                                                     cancelButtonItem:item3
                                                                destructiveButtonItem:item1
                                                                     otherButtonItems:item2, item3, item4,nil];

显示
    [action showInView:self.view];
