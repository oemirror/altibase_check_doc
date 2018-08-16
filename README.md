=================== README =================== 
1. 安装Python3
2. 安装相应的包
        docx  --> docx需要用whl安装，python_docx-0.8.6-py2.py3-none-any.whl
        os
        logging
        time
        json
        sys

3. 配置customer.json文件，格式如下：
    客户代码：BJ_UNICOM
        CUST_NAME ( 客户中文名 )：辽宁联通
        HOSTID_AITIBASEUSER（HOSTID_用户名称）: 0x84c22609_alti1
            MEM_DB_DIR0 ( 数据文件路径 )：/altibase_dbs0
            MEM_DB_DIR1 ( 数据文件路径 )：/altibase_dbs1
            MEM_LOG_DIR0 ( 数据文件路径 )：/altibase_log
    
    例如：   
    {
    "BJ_UNICOM":{"CUST_NAME":"北京联通",
    "0xF0DF5690_altibase":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x991B40A_altibase":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"}
    },
    "LN_UNICOM":{"CUST_NAME":"辽宁联通",
    "0x84c22609_alti1":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c22609_alti2":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c22609_alti3":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c22609_alti4":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c2260a_alti1":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c2260a_alti2":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c2260a_alti3":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c2260a_alti4":{"MEM_DB_DIR0":"/altibase_dbs0","MEM_DB_DIR1":"/altibase_dbs1","MEM_LOG_DIR0":"/altibase_log"},
    "0x84c2250d_alti01":{"MEM_DB_DIR0":"/alti01_data01","MEM_DB_DIR1":"/alti01_data02","MEM_LOG_DIR0":"/alti01_log01"},
    "0x84c2250d_alti02":{"MEM_DB_DIR0":"/alti01_data01","MEM_DB_DIR1":"/alti01_data02","MEM_LOG_DIR0":"/alti01_log01"},
    "0x84c2250d_alti03":{"MEM_DB_DIR0":"/alti01_data01","MEM_DB_DIR1":"/alti01_data02","MEM_LOG_DIR0":"/alti01_log01"},
    "0x84c2250f_alti01":{"MEM_DB_DIR0":"/alti01_data01","MEM_DB_DIR1":"/alti01_data02","MEM_LOG_DIR0":"/alti01_log01"},
    "0x84c2250f_alti02":{"MEM_DB_DIR0":"/alti01_data01","MEM_DB_DIR1":"/alti01_data02","MEM_LOG_DIR0":"/alti01_log01"},
    "0x84c2250f_alti03":{"MEM_DB_DIR0":"/alti01_data01","MEM_DB_DIR1":"/alti01_data02","MEM_LOG_DIR0":"/alti01_log01"}
    }
    }
    
4. 根目录放置上一次的巡检报告及本次的巡检日志文件

5. 执行docs.py 客户代码，比如：docs.py BJ_UNICOM

6. 根目录生成新的巡检报告

7. 查看CMD窗口REP_GAP，GC_GAP 判断复制和GC情况正常与否

8. 查看altibase_sm日志，确认checkpoint情况正常与否

9. 根据结果补充巡检分析总结 
   
