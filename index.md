/* 基础样式 */
#csbody {
    color: #F08080;  /* 全局文字颜色 */
    background-color: #f0fff0;
    font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
    line-height: 1.6;
    padding: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

/* 标题保持原有颜色 */
h2.section-title {
    color: #E6E6FA !important;  /* 强制保持标题颜色 */
    text-shadow: 2px 2px 0 #fff;
    position: relative;
    padding-left: 1.5rem;
    font-size: 2.2em;
    letter-spacing: 1px;
}

/* 呼号信息区块 */
#calldata {
    background: rgba(255, 255, 255, 0.9);
    color: inherit;  /* 继承全局文字颜色 */
    border-radius: 12px;
    padding: 2rem;
    margin: 2rem auto;
    width: 90%;
    box-shadow: 0 6px 12px rgba(0, 100, 0, 0.15);
    border-left: 5px solid #2e7d32;
}

/* 个人简介区块 */
#biodata {
    background-color: rgb(175, 238, 238);
    color: inherit;  /* 继承全局文字颜色 */
    border-radius: 10px;
    padding: 2rem;
    margin: 2rem auto;
    width: 92%;
    transform: perspective(1200px) rotateX(1deg);
    box-shadow: 0 4px 15px rgba(0, 100, 100, 0.2);
}

/* 调整首行文字颜色 */
#calldata::first-line,
#biodata::first-line,
#t_bio.biodiv::first-line {
    font-size: 1.4em;
    font-weight: 600;
    color: #1a237e;  /* 与全局颜色一致 */
    text-shadow: 1px 1px 0px rgba(0,0,0,0.3);  /* 调整阴影对比度 */
}

/* 表格内容 */
#t_bio.biodiv {
    background-color: #e0f7fa;
    color: inherit;  /* 继承全局颜色 */
    border: 2px dashed #26a69a;
    border-radius: 8px;
    padding: 1.5rem;
    margin: 1.5rem 0;
    width: 95%;
}

/* 链接保持独立颜色 */
a {
    color: #0d47a1;  /* 保持原有链接颜色 */
    text-decoration: none;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

a:hover {
    color: #d32f2f;
    text-decoration: underline wavy;
    text-underline-offset: 3px;
}

/* 响应式设计 */
@media (max-width: 768px) {
    #csbody {
        padding: 1.5rem;
        max-width: 95%;
    }
    
    #calldata, #biodata {
        width: 100%;
        margin: 1.5rem 0;
        border-radius: 8px;
    }
    
    h2.section-title {
        font-size: 1.8em;
    }
}
#t_bio.biodiv {background-color:#FFFFFF}
