# XCTestPlaygrounds

```swift 
import XCTest


struct APIClient {
  static func fetchData() -> String {
    return "data recieved"
  }
}


class TestApp: XCTestCase {
  
  func testFetchData() {
    let data = APIClient.fetchData()
    
    XCTAssertEqual(data, "data recieved", "not equal to 'data recieved'")
  }

}


TestApp.defaultTestSuite.run()
```
