## ReactJS Chapter 07
It is my coding practice with the TUTORIAL of Dave Gray. 

## Source
### Dave Gray 的 Reactjs 課程
https://youtube.com/playlist?list=PL0Zuz27SZ-6PrE9srvEn8nbhOOyxnWXfp
### Dave Gray 的 YouTube 頻道
https://www.youtube.com/@DaveGrayTeachesCode

## ReactJS Chapter 07
   Quick Concept outline
   中文摘要說明與重點提問

###  1. Intro 
        教學影片固定的開頭和摘要說明

###  2. Tutorial Setup <Code更動>
        修改刪除用不到的 Code

###  3. Changing the default state <Code更動>
        修改 array 的元素。
        將 useState 使用於新增的 array，array 中有三個 object。
        說明 object 中的 property 和 value 的資料型態。

###  4. View the new state in React Dev Tools
        檢視 Google 瀏覽器工具 Components 中
        Content 下層 state 的資料結構。

###  5. Displaying list items with map() <Code更動>
        使用 map 方法 新增三個有勾選功能的列表。
        列表的文字後方要新增刪除按鈕

        HTML: <ul></ul> <li></li> <input /> <label></label> <button></button>
              <??? className= "item"> <??? type="checkbox" checked={???}
        JavaScript: {item.map((item) => (???))} {???.checked}

###  6. Lists of elements need keys <Code更動>
        在 li 的 opening tag 設定 key，
        用來追蹤軌跡，識別項目是否被改變、加入或移除。
        
        HTML: <li></li>
              key= {???}
        JavaScript: {???.id}

###  7. Previewing the React list
        預覽列表目前的狀況
       
###  8. Adding the react-icons package <Code更動>
        在 npm 網站尋找 react 圖標的套件。
        在 git bash 執行指令安裝。
        套件安裝完成後匯入垃圾桶的圖標。
        移除刪除按鈕改為垃圾桶的圖標。

###  9. Applying CSS styles to the React list <Code更動>
        添加並說明 CSS 的樣式。
        勾選的 CSS 是哪個部分?
        垃圾桶的 CSS 是哪個部分?

### 10. Why we don't see a checkmark when we click <Code更動>
        示範如何透過修改 Code 勾選格子

### 11. Adding an onChange listener <Code更動>
        設定新的功能，放入參數，使列表的格子可以確認 key 的狀態。

        HTML: <??? onChange={???} />
        JavaScript: const handleCheck ......

### 12. The handleCheck function <Code更動>
        設定格子的勾選和取消勾選的功能，
        便能勾選與取消勾選。。

        JavaScript: const listItems ......

### 13. View the new component state in React Dev Tools
        檢視 Google 瀏覽器工具 Components 中
        Content 下層 state 的資料。

### 14. Saving state to localStorage
        將選單的項目存入 localStorage。

        JavaScript: localStorage ......

### 15. Adding an onDoubleClick listener
        設定雙重點擊選單的項目進行勾選或取消勾選。

        HTML: <??? onDoubleClick={???}>
        JavaScript: {???}

### 16. Adding conditional CSS styling
        設定打勾時，選單的項目會畫橫線；
        取消打勾時，選單項目橫線會消除。

        HTML: <??? style={???}>
        CSS: {???: "line-through"}
        JavaScript: {(???.checked) ...}

### 17. Adding an onClick listener
        暫時設定垃圾桶圖標的刪除功能為回傳 id。
        設定垃圾桶圖標刪除功能的參數。

        JavaScript: const handleDelete ...
        HTML: <??? onclick={???}>
        JavaScript: {???}

### 18. The handleDelete function
        將回傳 id 修改為刪除功能，
        點擊垃圾桶即可刪除選單:
        用 filter 新增 array
        將刪除選單的項目存入 localStorage

        JavaScript: const listItems ......
                    localStorage ......

### 19. Adding an empty list message
        當選單的項目全被刪除，
        顯示 Your list is empty.

        HTML: <ul>...</ul> <p style={}>Your list is empty.<p>
        CSS: marginTop: "2rem"
        JavaScript: ??? <ul>...</ul> ???

        Hint:
        (HTML element)
        {{CSS style}}
        {JavaScript expression}

### 20. When will we load state from localStorage?
        概述下一章的內容。


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
# ReactJS03QCo07
