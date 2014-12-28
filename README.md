OCUnit
======

单元测试学习
======

断言：
======
- XCTFail(format…) //生成一个失败的测试；
    
- XCTAssertNil(a1, format...)//为空判断，a1为空时通过，反之不通过；
    
- XCTAssertNotNil(a1, format…)//不为空判断，a1不为空时通过，反之不通过；
    
- XCTAssert(expression, format...)//当expression求值为TRUE时通过；
    
- XCTAssertTrue(expression, format...)//当expression求值为TRUE时通过；
    
- XCTAssertFalse(expression, format...)//当expression求值为False时通过；
    
- XCTAssertEqualObjects(a1, a2, format...)//判断相等，[a1 isEqual:a2]值为TRUE时通过，其中一个不为空时，不通过；
    
- XCTAssertNotEqualObjects(a1, a2, format...)//判断不等，[a1 isEqual:a2]值为False时通过；
    
- XCTAssertEqual(a1, a2, format...)//判断相等（当a1和a2是 C语言标量、结构体或联合体时使用,实际测试发现NSString也可以）；
    
- XCTAssertNotEqual(a1, a2, format...)//判断不等（当a1和a2是 C语言标量、结构体或联合体时使用）；
    
- XCTAssertEqualWithAccuracy(a1, a2, accuracy, format...)//判断相等，（double或float类型）提供一个误差范围，当在误差范围（+/-accuracy）以内相等时通过测试；
    
- XCTAssertNotEqualWithAccuracy(a1, a2, accuracy, format...)// 判断不等，（double或float类型）提供一个误差范围，当在误差范围以内不等时通过测试；
    
- XCTAssertThrows(expression, format...)//异常测试，当expression发生异常时通过；反之不通过；（很变态） XCTAssertThrowsSpecific(expression, specificException, format...) 异常测试，当expression发生specificException异常时通过；反之发生其他异常或不发生异常均不通过；
    
- XCTAssertThrowsSpecificNamed(expression, specificException, exception_name, format...)//异常测试，当expression发生具体异常、具体异常名称的异常时通过测试，反之不通过；
    
- XCTAssertNoThrow(expression, format…)//异常测试，当expression没有发生异常时通过测试；
    
- XCTAssertNoThrowSpecific(expression, specificException, format...)//异常测试，当expression没有发生具体异常、具体异常名称的异常时通过测试，反之不通过；
    
- XCTAssertNoThrowSpecificNamed(expression, specificException, exception_name, format...)//异常测试，当expression没有发生具体异常、具体异常名称的异常时通过测试，反之不通过

参考资料连接：
======
> Xcode5单元测试（一）使用XCTest进行单元测试：http://www.it165.net/pro/html/201403/10828.html


