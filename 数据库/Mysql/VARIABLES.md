# VARIABLES

## 命令解析

> 命令：`SHOW VARIABLES;`
> mysql官方文档：<https://dev.mysql.com/doc/refman/5.7/en/server-system-variables.html>

Variable_name | 变量名称 | Value
-- | -- | --
[auto_generate_certs](#auto_generate_certs) | 自动生成证书 | ON
[auto_increment_increment](#auto_increment_increment) | 自动递增增量 | 1
[auto_increment_offset](#auto_increment_offset) | 自动递增偏移 | 1
[autocommit](#autocommit) | 自动提交 | ON
[automatic_sp_privileges](#automatic_sp_privileges) | 自动sp特权 | ON
[avoid_temporal_upgrade](#avoid_temporal_upgrade) | 避免临时升级 | OFF
[back_log](#back_log) | 积压 | 80
[basedir](#basedir) | 根目录 | C:\Program Files\MySQL\MySQL Server 5.7\
[big_tables](#big_tables) | 大桌子 | OFF
[bind_address](#bind_address) | 绑定地址 | *
[binlog_cache_size](#binlog_cache_size) | binlog缓存大小 | 32768
[binlog_checksum](#binlog_checksum) | binlog校验和 | CRC32
[binlog_direct_non_transactional_updates](#binlog_direct_non_transactional_updates) | binlog直接非事务更新 | OFF
[binlog_error_action](#binlog_error_action) | binlog错误操作 | ABORT_SERVER
[binlog_format](#binlog_format) | binlog格式 | ROW
[binlog_group_commit_sync_delay](#binlog_group_commit_sync_delay) | binlog组提交同步延迟 | 0
[binlog_group_commit_sync_no_delay_count](#binlog_group_commit_sync_no_delay_count) | binlog组提交同步无延迟计数 | 0
[binlog_gtid_simple_recovery](#binlog_gtid_simple_recovery) | binlog-gtid简单恢复 | ON
[binlog_max_flush_queue_time](#binlog_max_flush_queue_time) | binlog最大刷新队列时间 | 0
[binlog_order_commits](#binlog_order_commits) | binlog订单提交 | ON
[binlog_row_image](#binlog_row_image) | binlog行图像 | FULL
[binlog_rows_query_log_events](#binlog_rows_query_log_events) | binlog行查询日志事件 | OFF
[binlog_stmt_cache_size](#binlog_stmt_cache_size) | binlog stmt缓存大小 | 32768
[binlog_transaction_dependency_history_size](#binlog_transaction_dependency_history_size) | binlog事务依赖关系历史记录大小 | 25000
[binlog_transaction_dependency_tracking](#binlog_transaction_dependency_tracking) | binlog事务依赖性跟踪 | COMMIT_ORDER
[block_encryption_mode](#block_encryption_mode) | 块加密模式 | aes-128-ecb
[bulk_insert_buffer_size](#bulk_insert_buffer_size) | 大容量插入缓冲区大小 | 8388608
[character_set_client](#character_set_client) | 字符集客户端 | utf8mb4
[character_set_connection](#character_set_connection) | 字符集连接 | utf8mb4
[character_set_database](#character_set_database) | 字符集数据库 | utf8mb4
[character_set_filesystem](#character_set_filesystem) | 字符集文件系统 | binary
[character_set_results](#character_set_results) | 字符集结果 | utf8mb4
[character_set_server](#character_set_server) | 字符集服务器 | latin1
[character_set_system](#character_set_system) | 字符集系统 | utf8
[character_sets_dir](#character_sets_dir) | 字符集目录 | C:\Program Files\MySQL\MySQL Server 5.7\share\charsets\
[check_proxy_users](#check_proxy_users) | 检查代理用户 | OFF
[collation_connection](#collation_connection) | 排序规则连接 | utf8mb4_general_ci
[collation_database](#collation_database) | 排序规则数据库 | utf8mb4_general_ci
[collation_server](#collation_server) | 排序规则服务器 | latin1_swedish_ci
[completion_type](#completion_type) | 完成类型 | NO_CHAIN
[concurrent_insert](#concurrent_insert) | 并行插入 | AUTO
[connect_timeout](#connect_timeout) | 连接超时 | 10
[core_file](#core_file) | 核心文件 | OFF
[datadir](#datadir) | 数据目录 | C:\ProgramData\MySQL\MySQL Server 5.7\Data\
[date_format](#date_format) | 日期格式 | %Y-%m-%d
[datetime_format](#datetime_format) | 日期时间格式 | %Y-%m-%d %H:%i:%s
[default_authentication_plugin](#default_authentication_plugin) | 默认身份验证插件 | mysql_native_password
[default_password_lifetime](#default_password_lifetime) | 默认密码生存期 | 0
[default_storage_engine](#default_storage_engine) | 默认存储引擎 | InnoDB
[default_tmp_storage_engine](#default_tmp_storage_engine) | 默认tmp存储引擎 | InnoDB
[default_week_format](#default_week_format) | 默认周格式 | 0
[delay_key_write](#delay_key_write) | 延迟键写入 | ON
[delayed_insert_limit](#delayed_insert_limit) | 延迟插入限制 | 100
[delayed_insert_timeout](#delayed_insert_timeout) | 延迟插入超时 | 300
[delayed_queue_size](#delayed_queue_size) | 延迟队列大小 | 1000
[disabled_storage_engines](#disabled_storage_engines) | 禁用的存储引擎 |
[disconnect_on_expired_password](#disconnect_on_expired_password) | 密码过期时断开连接 | ON
[div_precision_increment](#div_precision_increment) | div精度增量 | 4
[end_markers_in_json](#end_markers_in_json) | json中的结束标记 | OFF
[enforce_gtid_consistency](#enforce_gtid_consistency) | 强制gtid一致性 | OFF
[eq_range_index_dive_limit](#eq_range_index_dive_limit) | eq范围指数下降极限 | 200
[error_count](#error_count) | 错误计数 | 0
[event_scheduler](#event_scheduler) | 事件调度程序 | OFF
[expire_logs_days](#expire_logs_days) | 过期日志天数 | 0
[explicit_defaults_for_timestamp](#explicit_defaults_for_timestamp) | 时间戳的显式默认值 | OFF
[external_user](#external_user) | 外部用户 |
[flush](#flush) | 脸红 | OFF
[flush_time](#flush_time) | 冲洗时间 | 0
[foreign_key_checks](#foreign_key_checks) | 外键检查 | ON
[ft_boolean_syntax](#ft_boolean_syntax) | ft布尔语法 | + -><()~*:""&|
[ft_max_word_len](#ft_max_word_len) | ft最大字长度 | 84
[ft_min_word_len](#ft_min_word_len) | ft最小单词len | 4
[ft_query_expansion_limit](#ft_query_expansion_limit) | ft查询扩展限制 | 20
[ft_stopword_file](#ft_stopword_file) | ft停止字文件 | (built-in)
[general_log](#general_log) | 一般日志 | OFF
[general_log_file](#general_log_file) | 常规日志文件 | RAN.log
[group_concat_max_len](#group_concat_max_len) | 组concat最大len | 1024
[gtid_executed_compression_period](#gtid_executed_compression_period) | gtid执行的压缩周期 | 1000
[gtid_mode](#gtid_mode) | gtid模式 | OFF
[gtid_next](#gtid_next) | gtid下一个 | AUTOMATIC
[gtid_owned](#gtid_owned) | gtid拥有 |
[gtid_purged](#gtid_purged) | gtid已清除 |
[have_compress](#have_compress) | 有压缩 | YES
[have_crypt](#have_crypt) | 有crypt | NO
[have_dynamic_loading](#have_dynamic_loading) | 具有动态负载 | YES
[have_geometry](#have_geometry) | 具有几何图形 | YES
[have_openssl](#have_openssl) | 具有openssl | YES
[have_profiling](#have_profiling) | 具有配置文件 | YES
[have_query_cache](#have_query_cache) | 具有查询缓存 | YES
[have_rtree_keys](#have_rtree_keys) | 有rtree密钥 | YES
[have_ssl](#have_ssl) | 具有ssl | YES
[have_statement_timeout](#have_statement_timeout) | 有语句超时 | YES
[have_symlink](#have_symlink) | 具有符号链接 | YES
[host_cache_size](#host_cache_size) | 主机缓存大小 | 279
[hostname](#hostname) | 主机名 | ran
[identity](#identity) | 身份 | 0
[ignore_builtin_innodb](#ignore_builtin_innodb) | 忽略内置的innodb | OFF
[ignore_db_dirs](#ignore_db_dirs) | 忽略数据库目录 |
[init_connect](#init_connect) | 初始化连接 |
[init_file](#init_file) | init文件 |
[init_slave](#init_slave) | 初始化从机 |
[innodb_adaptive_flushing](#innodb_xxx) | innodb自适应冲洗 | ON
[innodb_adaptive_flushing_lwm](#innodb_xxx) | innodb自适应冲洗lwm | 10
[innodb_adaptive_hash_index](#innodb_xxx) | innodb自适应哈希索引 | ON
[innodb_adaptive_hash_index_parts](#innodb_xxx) | innodb自适应散列索引部分 | 8
[innodb_adaptive_max_sleep_delay](#innodb_xxx) | innodb自适应最大睡眠延迟 | 150000
[innodb_api_bk_commit_interval](#innodb_xxx) | innodb-api-bk提交间隔 | 5
[innodb_api_disable_rowlock](#innodb_xxx) | innodb api禁用rowlock | OFF
[innodb_api_enable_binlog](#innodb_xxx) | innodb-api启用binlog | OFF
[innodb_api_enable_mdl](#innodb_xxx) | innodb api启用mdl | OFF
[innodb_api_trx_level](#innodb_xxx) | innodb api trx级别 | 0
[innodb_autoextend_increment](#innodb_xxx) | innodb自动扩展增量 | 64
[innodb_autoinc_lock_mode](#innodb_xxx) | innodb autoinc锁定模式 | 1
[innodb_buffer_pool_chunk_size](#innodb_xxx) | innodb缓冲池块大小 | 134217728
[innodb_buffer_pool_dump_at_shutdown](#innodb_xxx) | innodb缓冲池在关闭时转储 | ON
[innodb_buffer_pool_dump_now](#innodb_xxx) | innodb缓冲池现在转储 | OFF
[innodb_buffer_pool_dump_pct](#innodb_xxx) | innodb缓冲池转储pct | 25
[innodb_buffer_pool_filename](#innodb_xxx) | innodb缓冲池文件名 | ib_buffer_pool
[innodb_buffer_pool_instances](#innodb_xxx) | innodb缓冲池实例 | 1
[innodb_buffer_pool_load_abort](#innodb_xxx) | innodb缓冲池加载中止 | OFF
[innodb_buffer_pool_load_at_startup](#innodb_xxx) | 启动时的innodb缓冲池加载 | ON
[innodb_buffer_pool_load_now](#innodb_xxx) | innodb缓冲池现在加载 | OFF
[innodb_buffer_pool_size](#innodb_xxx) | innodb缓冲池大小 | 134217728
[innodb_change_buffer_max_size](#innodb_xxx) | innodb更改缓冲区最大大小 | 25
[innodb_change_buffering](#innodb_xxx) | innodb更改缓冲 | all
[innodb_checksum_algorithm](#innodb_xxx) | innodb校验和算法 | crc32
[innodb_checksums](#innodb_xxx) | innodb校验和 | ON
[innodb_cmp_per_index_enabled](#innodb_xxx) | 已启用每个索引的innodb cmp | OFF
[innodb_commit_concurrency](#innodb_xxx) | innodb提交并发 | 0
[innodb_compression_failure_threshold_pct](#innodb_xxx) | innodb压缩失败阈值pct | 5
[innodb_compression_level](#innodb_xxx) | innodb压缩级别 | 6
[innodb_compression_pad_pct_max](#innodb_xxx) | innodb压缩垫pct最大值 | 50
[innodb_concurrency_tickets](#innodb_xxx) | innodb并发票证 | 5000
[innodb_data_file_path](#innodb_xxx) | innodb数据文件路径 | ibdata1:12M:autoextend
[innodb_data_home_dir](#innodb_xxx) | innodb数据主页目录 |
[innodb_deadlock_detect](#innodb_xxx) | innodb死锁检测 | ON
[innodb_default_row_format](#innodb_xxx) | innodb默认行格式 | dynamic
[innodb_disable_sort_file_cache](#innodb_xxx) | innodb禁用排序文件缓存 | OFF
[innodb_doublewrite](#innodb_xxx) | innodb双写 | ON
[innodb_fast_shutdown](#innodb_xxx) | innodb快速关闭 | 1
[innodb_file_format](#innodb_xxx) | innodb文件格式 | Barracuda
[innodb_file_format_check](#innodb_xxx) | innodb文件格式检查 | ON
[innodb_file_format_max](#innodb_xxx) | innodb文件格式最大值 | Barracuda
[innodb_file_per_table](#innodb_xxx) | 每个表的innodb文件 | ON
[innodb_fill_factor](#innodb_xxx) | innodb填充系数 | 100
[innodb_flush_log_at_timeout](#innodb_xxx) | innodb刷新日志超时 | 1
[innodb_flush_log_at_trx_commit](#innodb_xxx) | trx提交时的innodb刷新日志 | 1
[innodb_flush_method](#innodb_xxx) | innodb冲洗方法 |
[innodb_flush_neighbors](#innodb_xxx) | innodb刷新邻居 | 1
[innodb_flush_sync](#innodb_xxx) | innodb刷新同步 | ON
[innodb_flushing_avg_loops](#innodb_xxx) | innodb刷新avg循环 | 30
[innodb_force_load_corrupted](#innodb_xxx) | innodb强制负载已损坏 | OFF
[innodb_force_recovery](#innodb_xxx) | innodb力回收 | 0
[innodb_ft_aux_table](#innodb_xxx) | innodb ft aux表 |
[innodb_ft_cache_size](#innodb_xxx) | innodb-ft缓存大小 | 8000000
[innodb_ft_enable_diag_print](#innodb_xxx) | innodb-ft启用diag打印 | OFF
[innodb_ft_enable_stopword](#innodb_xxx) | innodb-ft启用停止字 | ON
[innodb_ft_max_token_size](#innodb_xxx) | innodb ft最大令牌大小 | 84
[innodb_ft_min_token_size](#innodb_xxx) | innodb ft最小令牌大小 | 3
[innodb_ft_num_word_optimize](#innodb_xxx) | innodb ft num字优化 | 2000
[innodb_ft_result_cache_limit](#innodb_xxx) | innodb-ft结果缓存限制 | 2000000000
[innodb_ft_server_stopword_table](#innodb_xxx) | innodb-ft服务器停止字表 |
[innodb_ft_sort_pll_degree](#innodb_xxx) | innodb-ft排序pll度 | 2
[innodb_ft_total_cache_size](#innodb_xxx) | innodb-ft缓存总大小 | 640000000
[innodb_ft_user_stopword_table](#innodb_xxx) | innodb-ft用户停止字表 |
[innodb_io_capacity](#innodb_xxx) | innodb-io容量 | 200
[innodb_io_capacity_max](#innodb_xxx) | innodb-io最大容量 | 2000
[innodb_large_prefix](#innodb_xxx) | innodb大前缀 | ON
[innodb_lock_wait_timeout](#innodb_xxx) | innodb锁等待超时 | 50
[innodb_locks_unsafe_for_binlog](#innodb_xxx) | innodb锁对binlog不安全 | OFF
[innodb_log_buffer_size](#innodb_xxx) | innodb日志缓冲区大小 | 16777216
[innodb_log_checksums](#innodb_xxx) | innodb日志校验和 | ON
[innodb_log_compressed_pages](#innodb_xxx) | innodb日志压缩页面 | ON
[innodb_log_file_size](#innodb_xxx) | innodb日志文件大小 | 50331648
[innodb_log_files_in_group](#innodb_xxx) | 组中的innodb日志文件 | 2
[innodb_log_group_home_dir](#innodb_xxx) | innodb日志组主目录 | .\
[innodb_log_write_ahead_size](#innodb_xxx) | innodb日志提前写入大小 | 8192
[innodb_lru_scan_depth](#innodb_xxx) | innodb-lru扫描深度 | 1024
[innodb_max_dirty_pages_pct](#innodb_xxx) | innodb最大脏页pct | 75
[innodb_max_dirty_pages_pct_lwm](#innodb_xxx) | innodb最大脏页pct-lwm | 0
[innodb_max_purge_lag](#innodb_xxx) | innodb最大清除滞后 | 0
[innodb_max_purge_lag_delay](#innodb_xxx) | innodb最大清除滞后延迟 | 0
[innodb_max_undo_log_size](#innodb_xxx) | innodb最大撤消日志大小 | 1073741824
[innodb_monitor_disable](#innodb_xxx) | innodb监视器禁用 |
[innodb_monitor_enable](#innodb_xxx) | innodb监视器启用 |
[innodb_monitor_reset](#innodb_xxx) | innodb监视器重置 |
[innodb_monitor_reset_all](#innodb_xxx) | innodb监视器全部重置 |
[innodb_old_blocks_pct](#innodb_xxx) | innodb旧块pct | 37
[innodb_old_blocks_time](#innodb_xxx) | innodb旧块时间 | 1000
[innodb_online_alter_log_max_size](#innodb_xxx) | innodb在线更改日志最大大小 | 134217728
[innodb_open_files](#innodb_xxx) | innodb打开文件 | 2000
[innodb_optimize_fulltext_only](#innodb_xxx) | innodb仅优化全文 | OFF
[innodb_page_cleaners](#innodb_xxx) | innodb页面清洁器 | 1
[innodb_page_size](#innodb_xxx) | innodb页面大小 | 16384
[innodb_print_all_deadlocks](#innodb_xxx) | innodb打印所有死锁 | OFF
[innodb_purge_batch_size](#innodb_xxx) | innodb清除批量大小 | 300
[innodb_purge_rseg_truncate_frequency](#innodb_xxx) | innodb清除rseg截断频率 | 128
[innodb_purge_threads](#innodb_xxx) | innodb清除线程 | 4
[innodb_random_read_ahead](#innodb_xxx) | innodb随机预读 | OFF
[innodb_read_ahead_threshold](#innodb_xxx) | innodb预读阈值 | 56
[innodb_read_io_threads](#innodb_xxx) | innodb读取io线程 | 4
[innodb_read_only](#innodb_xxx) | innodb只读 | OFF
[innodb_replication_delay](#innodb_xxx) | innodb复制延迟 | 0
[innodb_rollback_on_timeout](#innodb_xxx) | innodb超时回滚 | OFF
[innodb_rollback_segments](#innodb_xxx) | innodb回滚段 | 128
[innodb_sort_buffer_size](#innodb_xxx) | innodb排序缓冲区大小 | 1048576
[innodb_spin_wait_delay](#innodb_xxx) | innodb旋转等待延迟 | 6
[innodb_stats_auto_recalc](#innodb_xxx) | innodb统计自动重新计算 | ON
[innodb_stats_include_delete_marked](#innodb_xxx) | innodb统计信息包括已标记的删除 | OFF
[innodb_stats_method](#innodb_xxx) | innodb-stats方法 | nulls_equal
[innodb_stats_on_metadata](#innodb_xxx) | innodb元数据统计信息 | OFF
[innodb_stats_persistent](#innodb_xxx) | innodb统计数据持久 | ON
[innodb_stats_persistent_sample_pages](#innodb_xxx) | innodb统计持久样本页 | 20
[innodb_stats_sample_pages](#innodb_xxx) | innodb统计数据示例页 | 8
[innodb_stats_transient_sample_pages](#innodb_xxx) | innodb统计瞬态示例页 | 8
[innodb_status_output](#innodb_xxx) | innodb状态输出 | OFF
[innodb_status_output_locks](#innodb_xxx) | innodb状态输出锁 | OFF
[innodb_strict_mode](#innodb_xxx) | innodb严格模式 | ON
[innodb_support_xa](#innodb_xxx) | innodb支持xa | ON
[innodb_sync_array_size](#innodb_xxx) | innodb同步数组大小 | 1
[innodb_sync_spin_loops](#innodb_xxx) | innodb同步旋转循环 | 30
[innodb_table_locks](#innodb_xxx) | innodb表锁 | ON
[innodb_temp_data_file_path](#innodb_xxx) | innodb临时数据文件路径 | ibtmp1:12M:autoextend
[innodb_thread_concurrency](#innodb_xxx) | innodb线程并发 | 33
[innodb_thread_sleep_delay](#innodb_xxx) | innodb线程睡眠延迟 | 0
[innodb_tmpdir](#innodb_xxx) | innodb-tmpdir |
[innodb_undo_directory](#innodb_xxx) | innodb undo目录 | .\
[innodb_undo_log_truncate](#innodb_xxx) | innodb撤消日志截断 | OFF
[innodb_undo_logs](#innodb_xxx) | innodb撤消日志 | 128
[innodb_undo_tablespaces](#innodb_xxx) | innodb撤消表空间 | 0
[innodb_use_native_aio](#innodb_xxx) | innodb使用原生aio | ON
[innodb_version](#innodb_xxx) | innodb版本 | 5.7.40
[innodb_write_io_threads](#innodb_xxx) | innodb写入io线程 | 4
[insert_id](#insert_id) | 插入id | 0
[interactive_timeout](#interactive_timeout) | 交互式超时 | 28800
[internal_tmp_disk_storage_engine](#internal_tmp_disk_storage_engine) | 内部tmp磁盘存储引擎 | InnoDB
[join_buffer_size](#join_buffer_size) | 联接缓冲区大小 | 262144
[keep_files_on_create](#keep_files_on_create) | 保持文件处于创建状态 | OFF
[key_buffer_size](#key_buffer_size) | 密钥缓冲区大小 | 8388608
[key_cache_age_threshold](#key_cache_age_threshold) | 密钥缓存使用期限阈值 | 300
[key_cache_block_size](#key_cache_block_size) | 密钥缓存块大小 | 1024
[key_cache_division_limit](#key_cache_division_limit) | 密钥缓存划分限制 | 100
[keyring_operations](#keyring_operations) | 钥匙圈操作 | ON
[large_files_support](#large_files_support) | 大文件支持 | ON
[large_page_size](#large_page_size) | 大页面大小 | 0
[large_pages](#large_pages) | 大页面 | OFF
[last_insert_id](#last_insert_id) | 上次插入id | 0
[lc_messages](#lc_messages) | lc消息 | en_US
[lc_messages_dir](#lc_messages_dir) | lc消息目录 | C:\Program Files\MySQL\MySQL Server 5.7\share\
[lc_time_names](#lc_time_names) | lc时间名称 | en_US
[license](#license) | 许可证 | GPL
[local_infile](#local_infile) | 局部内野 | ON
[lock_wait_timeout](#lock_wait_timeout) | 锁定等待超时 | 31536000
[log_bin](#log_bin) | 原木仓位 | OFF
[log_bin_basename](#log_bin) | 日志箱基本名称 |
[log_bin_index](#log_bin) | 原木箱索引 |
[log_bin_trust_function_creators](#log_bin) | log-bin信任函数创建者 | OFF
[log_bin_use_v1_row_events](#log_bin) | 记录bin使用v1行事件 | OFF
[log_builtin_as_identified_by_password](#log_bin) | 通过密码标识的日志内置 | OFF
[log_error](#log_error) | 日志错误 | .\RAN.err
[log_error_verbosity](#log_error_verbosity) | 日志错误详细程度 | 3
[log_output](#log_output) | 日志输出 | FILE
[log_queries_not_using_indexes](#log_queries_not_using_indexes) | 不使用索引的日志查询 | OFF
[log_slave_updates](#log_slave_updates) | 日志从属更新 | OFF
[log_slow_admin_statements](#log_slow_admin_statements) | 记录慢速管理语句 | OFF
[log_slow_slave_statements](#log_slow_slave_statements) | 记录慢速从属语句 | OFF
[log_statements_unsafe_for_binlog](#log_statements_unsafe_for_binlog) | 日志语句对binlog不安全 | ON
[log_syslog](#log_syslog) | 日志系统日志 | ON
[log_syslog_tag](#log_syslog_tag) | log syslog标记 |
[log_throttle_queries_not_using_indexes](#log_throttle_queries_not_using_indexes) | 不使用索引的日志限制查询 | 0
[log_timestamps](#log_timestamps) | 日志时间戳 | UTC
[log_warnings](#log_warnings) | 日志警告 | 2
[long_query_time](#long_query_time) | 查询时间长 | 10
[low_priority_updates](#low_priority_updates) | 低优先级更新 | OFF
[lower_case_file_system](#lower_case_file_system) | 小写文件系统 | ON
[lower_case_table_names](#lower_case_table_names) | 小写表格名称 | 1
[master_info_repository](#master_info_repository) | 主信息存储库 | FILE
[master_verify_checksum](#master_verify_checksum) | 主校验和 | OFF
[max_allowed_packet](#max_allowed_packet) | 最大允许数据包 | 4194304
[max_binlog_cache_size](#max_binlog_cache_size) | binlog缓存的最大大小 | 1.84467E+19
[max_binlog_size](#max_binlog_size) | 最大binlog大小 | 1073741824
[max_binlog_stmt_cache_size](#max_binlog_stmt_cache_size) | 最大binlog stmt缓存大小 | 1.84467E+19
[max_connect_errors](#max_connect_errors) | 最大连接错误 | 100
[max_connections](#max_connections) | 最大连接数 | 151
[max_delayed_threads](#max_delayed_threads) | 最大延迟线程数 | 20
[max_digest_length](#max_digest_length) | 最大摘要长度 | 1024
[max_error_count](#max_error_count) | 最大错误计数 | 64
[max_execution_time](#max_execution_time) | 最大执行时间 | 0
[max_heap_table_size](#max_heap_table_size) | 最大堆表大小 | 16777216
[max_insert_delayed_threads](#max_insert_delayed_threads) | 最大插入延迟线程数 | 20
[max_join_size](#max_join_size) | 最大联接大小 | 1.84467E+19
[max_length_for_sort_data](#max_length_for_sort_data) | 排序数据的最大长度 | 1024
[max_points_in_geometry](#max_points_in_geometry) | 几何图形中的最大点 | 65536
[max_prepared_stmt_count](#max_prepared_stmt_count) | 最大准备stmt计数 | 16382
[max_relay_log_size](#max_relay_log_size) | 最大中继日志大小 | 0
[max_seeks_for_key](#max_seeks_for_key) | max寻找密钥 | 4294967295
[max_sort_length](#max_sort_length) | 最大排序长度 | 1024
[max_sp_recursion_depth](#max_sp_recursion_depth) | 最大sp递归深度 | 0
[max_tmp_tables](#max_tmp_tables) | 最大tmp表 | 32
[max_user_connections](#max_user_connections) | 最大用户连接数 | 0
[max_write_lock_count](#max_write_lock_count) | 最大写入锁定计数 | 4294967295
[metadata_locks_cache_size](#metadata_locks_cache_size) | 元数据锁定缓存大小 | 1024
[metadata_locks_hash_instances](#metadata_locks_hash_instances) | 元数据锁定哈希实例 | 8
[min_examined_row_limit](#min_examined_row_limit) | 最小检查行限制 | 0
[multi_range_count](#multi_range_count) | 多量程计数 | 256
[myisam_data_pointer_size](#myisam_data_pointer_size) | myisam数据指针大小 | 6
[myisam_max_sort_file_size](#myisam_max_sort_file_size) | myisam最大排序文件大小 | 1.07374E+11
[myisam_mmap_size](#myisam_mmap_size) | myisam mmap大小 | 1.84467E+19
[myisam_recover_options](#myisam_recover_options) | myisam恢复选项 | OFF
[myisam_sort_buffer_size](#myisam_sort_buffer_size) | myisam排序缓冲区大小 | 145752064
[myisam_stats_method](#myisam_stats_method) | myisam统计方法 | nulls_unequal
[myisam_use_mmap](#myisam_use_mmap) | myisam使用mmap | OFF
[mysql_native_password_proxy_users](#mysql_native_password_proxy_users) | mysql本机密码代理用户 | OFF
[named_pipe](#named_pipe) | 命名管道 | OFF
[named_pipe_full_access_group](#named_pipe_full_access_group) | 命名管道完全访问组 |
[net_buffer_length](#net_buffer_length) | 净缓冲区长度 | 16384
[net_read_timeout](#net_read_timeout) | 网络读取超时 | 30
[net_retry_count](#net_retry_count) | 净重试计数 | 10
[net_write_timeout](#net_write_timeout) | 网络写入超时 | 60
[new](#new) | 新 | OFF
[ngram_token_size](#ngram_token_size) | ngram令牌大小 | 2
[offline_mode](#offline_mode) | 脱机模式 | OFF
[old](#old) | 老的 | OFF
[old_alter_table](#old_alter_table) | 旧的替换表 | OFF
[old_passwords](#old_passwords) | 旧密码 | 0
[open_files_limit](#open_files_limit) | 打开文件限制 | 6209
[optimizer_prune_level](#optimizer_prune_level) | 优化器修剪级别 | 1
[optimizer_search_depth](#optimizer_search_depth) | 优化器搜索深度 | 62
[optimizer_switch](#optimizer_switch) | 优化器开关 | index_merge=on,index_merge_union=on,index_merge_sort_union=on,index_merge_intersection=on,engine_condition_pushdown=on,index_condition_pushdown=on,mrr=on,mrr_cost_based=on,block_nested_loop=on,batched_key_access=off,materialization=on,semijoin=on,loosescan=on,firstmatch=on,duplicateweedout=on,subquery_materialization_cost_based=on,use_index_extensions=on,condition_fanout_filter=on,derived_merge=on,prefer_ordering_index=on
[optimizer_trace](#optimizer_trace) | 优化器跟踪 | enabled=off,one_line=off
[optimizer_trace_features](#optimizer_trace_features) | 优化器跟踪功能 | greedy_search=on,range_optimizer=on,dynamic_range=on,repeated_subselect=on
[optimizer_trace_limit](#optimizer_trace_limit) | 优化器跟踪限制 | 1
[optimizer_trace_max_mem_size](#optimizer_trace_max_mem_size) | 优化器跟踪最大内存大小 | 16384
[optimizer_trace_offset](#optimizer_trace_offset) | 优化器跟踪偏移 | -1
[parser_max_mem_size](#parser_max_mem_size) | 解析器最大内存大小 | 1.84467E+19
[performance_schema](#performance_schema) | 性能模式 | ON
[performance_schema_accounts_size](#performance_schema_accounts_size) | 性能架构帐户大小 | -1
[performance_schema_digests_size](#performance_schema_digests_size) | 性能模式摘要大小 | 10000
[performance_schema_events_stages_history_long_size](#performance_schema_events_stages_history_long_size) | 性能模式事件阶段历史悠久 | 10000
[performance_schema_events_stages_history_size](#performance_schema_events_stages_history_size) | 性能架构事件阶段历史记录大小 | 10
[performance_schema_events_statements_history_long_size](#performance_schema_events_statements_history_long_size) | 性能模式事件语句历史悠久 | 10000
[performance_schema_events_statements_history_size](#performance_schema_events_statements_history_size) | 性能架构事件语句历史记录大小 | 10
[performance_schema_events_transactions_history_long_size](#performance_schema_events_transactions_history_long_size) | 性能架构事件事务历史悠久 | 10000
[performance_schema_events_transactions_history_size](#performance_schema_events_transactions_history_size) | 性能架构事件事务历史记录大小 | 10
[performance_schema_events_waits_history_long_size](#performance_schema_events_waits_history_long_size) | 性能架构事件等待历史悠久 | 10000
[performance_schema_events_waits_history_size](#performance_schema_events_waits_history_size) | 性能架构事件等待历史记录大小 | 10
[performance_schema_hosts_size](#performance_schema_hosts_size) | 性能架构主机大小 | -1
[performance_schema_max_cond_classes](#performance_schema_max_cond_classes) | 性能架构最大cond类 | 80
[performance_schema_max_cond_instances](#performance_schema_max_cond_instances) | 性能架构最大秒实例 | -1
[performance_schema_max_digest_length](#performance_schema_max_digest_length) | 性能架构最大摘要长度 | 1024
[performance_schema_max_file_classes](#performance_schema_max_file_classes) | 性能架构最大文件类 | 80
[performance_schema_max_file_handles](#performance_schema_max_file_handles) | 性能架构最大文件句柄 | 32768
[performance_schema_max_file_instances](#performance_schema_max_file_instances) | 性能架构最大文件实例数 | -1
[performance_schema_max_index_stat](#performance_schema_max_index_stat) | 性能架构最大索引stat | -1
[performance_schema_max_memory_classes](#performance_schema_max_memory_classes) | 性能架构最大内存类 | 320
[performance_schema_max_metadata_locks](#performance_schema_max_metadata_locks) | 性能架构最大元数据锁 | -1
[performance_schema_max_mutex_classes](#performance_schema_max_mutex_classes) | 性能模式最大互斥类 | 210
[performance_schema_max_mutex_instances](#performance_schema_max_mutex_instances) | 性能模式最大互斥实例数 | -1
[performance_schema_max_prepared_statements_instances](#performance_schema_max_prepared_statements_instances) | 性能架构最大准备语句实例 | -1
[performance_schema_max_program_instances](#performance_schema_max_program_instances) | 性能架构最大程序实例 | -1
[performance_schema_max_rwlock_classes](#performance_schema_max_rwlock_classes) | 性能模式最大rwlock类 | 50
[performance_schema_max_rwlock_instances](#performance_schema_max_rwlock_instances) | 性能架构最大rwlock实例 | -1
[performance_schema_max_socket_classes](#performance_schema_max_socket_classes) | 性能架构最大套接字类 | 10
[performance_schema_max_socket_instances](#performance_schema_max_socket_instances) | 性能架构最大套接字实例数 | -1
[performance_schema_max_sql_text_length](#performance_schema_max_sql_text_length) | 性能模式最大sql文本长度 | 1024
[performance_schema_max_stage_classes](#performance_schema_max_stage_classes) | 性能架构最大阶段类 | 150
[performance_schema_max_statement_classes](#performance_schema_max_statement_classes) | 性能架构最大语句类 | 193
[performance_schema_max_statement_stack](#performance_schema_max_statement_stack) | 性能模式最大语句堆栈 | 10
[performance_schema_max_table_handles](#performance_schema_max_table_handles) | 性能架构最大表句柄 | -1
[performance_schema_max_table_instances](#performance_schema_max_table_instances) | 性能架构最大表实例数 | -1
[performance_schema_max_table_lock_stat](#performance_schema_max_table_lock_stat) | 性能架构最大表锁定stat | -1
[performance_schema_max_thread_classes](#performance_schema_max_thread_classes) | 性能架构最大线程类 | 50
[performance_schema_max_thread_instances](#performance_schema_max_thread_instances) | 性能架构最大线程实例数 | -1
[performance_schema_session_connect_attrs_size](#performance_schema_session_connect_attrs_size) | 性能架构会话连接属性大小 | 512
[performance_schema_setup_actors_size](#performance_schema_setup_actors_size) | 性能模式设置参与者大小 | -1
[performance_schema_setup_objects_size](#performance_schema_setup_objects_size) | 性能架构设置对象大小 | -1
[performance_schema_show_processlist](#performance_schema_show_processlist) | 性能模式显示进程列表 | OFF
[performance_schema_users_size](#performance_schema_users_size) | 性能架构用户大小 | -1
[pid_file](#pid_file) | pid文件 | C:\ProgramData\MySQL\MySQL Server 5.7\Data\ran.pid
[plugin_dir](#plugin_dir) | 插件目录 | C:\Program Files\MySQL\MySQL Server 5.7\lib\plugin\
[port](#port) | 港口城市 | 3306
[preload_buffer_size](#preload_buffer_size) | 预加载缓冲区大小 | 32768
[profiling](#profiling) | 剖析 | ON
[profiling_history_size](#profiling_history_size) | 分析历史记录大小 | 15
[protocol_version](#protocol_version) | 协议版本 | 10
[proxy_user](#proxy_user) | 代理用户 |
[pseudo_slave_mode](#pseudo_slave_mode) | 伪从属模式 | OFF
[pseudo_thread_id](#pseudo_thread_id) | 伪线程id | 3
[query_alloc_block_size](#query_alloc_block_size) | 查询分配块大小 | 8192
[query_cache_limit](#query_cache_limit) | 查询缓存限制 | 1048576
[query_cache_min_res_unit](#query_cache_min_res_unit) | 查询缓存最小res单位 | 4096
[query_cache_size](#query_cache_size) | 查询缓存大小 | 1048576
[query_cache_type](#query_cache_type) | 查询缓存类型 | OFF
[query_cache_wlock_invalidate](#query_cache_wlock_invalidate) | 查询缓存wlock无效 | OFF
[query_prealloc_size](#query_prealloc_size) | 查询前缀大小 | 8192
[rand_seed1](#rand_seed1) | 兰特种子1 | 0
[rand_seed2](#rand_seed2) | 兰特种子2 | 0
[range_alloc_block_size](#range_alloc_block_size) | 范围分配块大小 | 4096
[range_optimizer_max_mem_size](#range_optimizer_max_mem_size) | 范围优化器最大内存大小 | 8388608
[rbr_exec_mode](#rbr_exec_mode) | rbr执行模式 | STRICT
[read_buffer_size](#read_buffer_size) | 读取缓冲区大小 | 65536
[read_only](#read_only) | 只读 | OFF
[read_rnd_buffer_size](#read_rnd_buffer_size) | 读取rnd缓冲区大小 | 262144
[relay_log](#relay_log) | 继电器日志 |
[relay_log_basename](#relay_log_basename) | 中继日志基名称 | C:\ProgramData\MySQL\MySQL Server 5.7\Data\ran-relay-bin
[relay_log_index](#relay_log_index) | 中继日志索引 | C:\ProgramData\MySQL\MySQL Server 5.7\Data\ran-relay-bin.index
[relay_log_info_file](#relay_log_info_file) | 中继日志信息文件 | relay-log.info
[relay_log_info_repository](#relay_log_info_repository) | 中继日志信息存储库 | FILE
[relay_log_purge](#relay_log_purge) | 中继日志清除 | ON
[relay_log_recovery](#relay_log_recovery) | 中继日志恢复 | OFF
[relay_log_space_limit](#relay_log_space_limit) | 继电器日志空间限制 | 0
[replication_optimize_for_static_plugin_config](#replication_optimize_for_static_plugin_config) | 针对静态插件配置的复制优化 | OFF
[replication_sender_observe_commit_only](#replication_sender_observe_commit_only) | 复制发送方仅观察提交 | OFF
[report_host](#report_host) | 报表主机 |
[report_password](#report_password) | 报表密码 |
[report_port](#report_port) | 报告端口 | 3306
[report_user](#report_user) | 报表用户 |
[require_secure_transport](#require_secure_transport) | 需要安全运输 | OFF
[rpl_stop_slave_timeout](#rpl_stop_slave_timeout) | rpl停止从属超时 | 31536000
[secure_auth](#secure_auth) | 安全身份验证 | ON
[secure_file_priv](#secure_file_priv) | 安全文件priv | C:\ProgramData\MySQL\MySQL Server 5.7\Uploads\
[server_id](#server_id) | 服务器id | 1
[server_id_bits](#server_id_bits) | 服务器id位 | 32
[server_uuid](#server_uuid) | 服务器uuid | 33d2e322-d3b6-11ed-a7e1-c82355424cb6
[session_track_gtids](#session_track_gtids) | 会话跟踪gtid | OFF
[session_track_schema](#session_track_schema) | 会话跟踪模式 | ON
[session_track_state_change](#session_track_state_change) | 会话跟踪状态更改 | OFF
[session_track_system_variables](#session_track_system_variables) | 会话跟踪系统变量 | time_zone,autocommit,character_set_client,character_set_results,character_set_connection
[session_track_transaction_info](#session_track_transaction_info) | 会话跟踪事务信息 | OFF
[sha256_password_auto_generate_rsa_keys](#sha256_password_auto_generate_rsa_keys) | sha256密码自动生成rsa密钥 | ON
[sha256_password_private_key_path](#sha256_password_private_key_path) | sha256密码私钥路径 | private_key.pem
[sha256_password_proxy_users](#sha256_password_proxy_users) | sha256密码代理用户 | OFF
[sha256_password_public_key_path](#sha256_password_public_key_path) | sha256密码公钥路径 | public_key.pem
[shared_memory](#shared_memory) | 共享存储器 | OFF
[shared_memory_base_name](#shared_memory_base_name) | 共享内存基本名称 | MYSQL
[show_compatibility_56](#show_compatibility_56) | 显示兼容性56 | OFF
[show_create_table_verbosity](#show_create_table_verbosity) | 显示创建表的详细信息 | OFF
[show_old_temporals](#show_old_temporals) | 显示旧时态 | OFF
[skip_external_locking](#skip_external_locking) | 跳过外部锁定 | ON
[skip_name_resolve](#skip_name_resolve) | 跳过名称解析 | OFF
[skip_networking](#skip_networking) | 跳过网络 | OFF
[skip_show_database](#skip_show_database) | 跳过显示数据库 | OFF
[slave_allow_batching](#slave_allow_batching) | 从允许批处理 | OFF
[slave_checkpoint_group](#slave_checkpoint_group) | 从属检查点组 | 512
[slave_checkpoint_period](#slave_checkpoint_period) | 从检查点周期 | 300
[slave_compressed_protocol](#slave_compressed_protocol) | 从压缩协议 | OFF
[slave_exec_mode](#slave_exec_mode) | 从执行模式 | STRICT
[slave_load_tmpdir](#slave_load_tmpdir) | 从负载tmpdir | C:\Windows\SERVIC~1\NETWOR~1\AppData\Local\Temp
[slave_max_allowed_packet](#slave_max_allowed_packet) | 从设备允许的最大数据包 | 1073741824
[slave_net_timeout](#slave_net_timeout) | 从网超时 | 60
[slave_parallel_type](#slave_parallel_type) | 从并行型 | DATABASE
[slave_parallel_workers](#slave_parallel_workers) | 奴隶平行工人 | 0
[slave_pending_jobs_size_max](#slave_pending_jobs_size_max) | 从属挂起作业最大大小 | 16777216
[slave_preserve_commit_order](#slave_preserve_commit_order) | 从保留提交顺序 | OFF
[slave_rows_search_algorithms](#slave_rows_search_algorithms) | 从行搜索算法 | TABLE_SCAN,INDEX_SCAN
[slave_skip_errors](#slave_skip_errors) | 从属跳过错误 | OFF
[slave_sql_verify_checksum](#slave_sql_verify_checksum) | 从sql验证校验和 | ON
[slave_transaction_retries](#slave_transaction_retries) | 从属事务重试次数 | 10
[slave_type_conversions](#slave_type_conversions) | 从类型转换 |
[slow_launch_time](#slow_launch_time) | 发射时间慢 | 2
[slow_query_log](#slow_query_log) | 慢速查询日志 | ON
[slow_query_log_file](#slow_query_log_file) | 慢速查询日志文件 | RAN-slow.log
[socket](#socket) | 插座 | MySQL
[sort_buffer_size](#sort_buffer_size) | 排序缓冲区大小 | 262144
[sql_auto_is_null](#sql_auto_is_null) | sql auto为null | OFF
[sql_big_selects](#sql_big_selects) | sql大选择 | ON
[sql_buffer_result](#sql_buffer_result) | sql缓冲区结果 | OFF
[sql_log_bin](#sql_log_bin) | sql日志箱 | ON
[sql_log_off](#sql_log_off) | sql注销 | OFF
[sql_mode](#sql_mode) | sql模式 | STRICT_TRANS_TABLES,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION
[sql_notes](#sql_notes) | sql注释 | ON
[sql_quote_show_create](#sql_quote_show_create) | sql报价显示创建 | ON
[sql_safe_updates](#sql_safe_updates) | sql安全更新 | OFF
[sql_select_limit](#sql_select_limit) | sql选择限制 | 1.84467E+19
[sql_slave_skip_counter](#sql_slave_skip_counter) | sql从跳过计数器 | 0
[sql_warnings](#sql_warnings) | sql警告 | OFF
[ssl_ca](#ssl_ca) | ssl ca | ca.pem
[ssl_capath](#ssl_capath) | ssl容量 |
[ssl_cert](#ssl_cert) | ssl证书 | server-cert.pem
[ssl_cipher](#ssl_cipher) | ssl密码 |
[ssl_crl](#ssl_crl) | ssl crl |
[ssl_crlpath](#ssl_crlpath) | ssl crlpath |
[ssl_key](#ssl_key) | ssl密钥 | server-key.pem
[stored_program_cache](#stored_program_cache) | 存储程序缓存 | 256
[super_read_only](#super_read_only) | 超级只读 | OFF
[sync_binlog](#sync_binlog) | 同步binlog | 1
[sync_frm](#sync_frm) | 同步frm | ON
[sync_master_info](#sync_master_info) | 同步主信息 | 10000
[sync_relay_log](#sync_relay_log) | 同步中继日志 | 10000
[sync_relay_log_info](#sync_relay_log_info) | 同步中继日志信息 | 10000
[system_time_zone](#system_time_zone) | 系统时区 |
[table_definition_cache](#table_definition_cache) | 表定义缓存 | 1400
[table_open_cache](#table_open_cache) | 表打开缓存 | 2000
[table_open_cache_instances](#table_open_cache_instances) | 表打开缓存实例 | 16
[thread_cache_size](#thread_cache_size) | 线程缓存大小 | 10
[thread_handling](#thread_handling) | 线程处理 | one-thread-per-connection
[thread_stack](#thread_stack) | 线程堆栈 | 262144
[time_format](#time_format) | 时间格式 | %H:%i:%s
[time_zone](#time_zone) | 时区 | SYSTEM
[timestamp](#timestamp) | 时间戳 | 1704764877
[tls_version](#tls_version) | tls版本 | TLSv1,TLSv1.1,TLSv1.2
[tmp_table_size](#tmp_table_size) | tmp表大小 | 77594624
[tmpdir](#tmpdir) | tmpdir | C:\Windows\SERVIC~1\NETWOR~1\AppData\Local\Temp
[transaction_alloc_block_size](#transaction_alloc_block_size) | 事务分配块大小 | 8192
[transaction_allow_batching](#transaction_allow_batching) | 事务允许批处理 | OFF
[transaction_isolation](#transaction_isolation) | 事务隔离 | REPEATABLE-READ
[transaction_prealloc_size](#transaction_prealloc_size) | 事务预分配大小 | 4096
[transaction_read_only](#transaction_read_only) | 事务只读 | OFF
[transaction_write_set_extraction](#transaction_write_set_extraction) | 事务写入集提取 | OFF
[tx_isolation](#tx_isolation) | tx隔离 | REPEATABLE-READ
[tx_read_only](#tx_read_only) | tx只读 | OFF
[unique_checks](#unique_checks) | 唯一的检查 | ON
[updatable_views_with_limit](#updatable_views_with_limit) | 带限制的可更新视图 | YES
[version](#version) | 版本 | 5.7.40-log
[version_comment](#version_comment) | 版本注释 | MySQL Community Server (GPL)
[version_compile_machine](#version_compile_machine) | 版本编译机 | x86_64
[version_compile_os](#version_compile_os) | 版本编译操作系统 | Win64
[wait_timeout](#wait_timeout) | 等待超时 | 28800
[warning_count](#warning_count) | 警告计数 | 0

## auto_generate_certs

> **自动生成证书**

`auto_generate_certs` 是一个与`SSL/TLS`证书相关的配置参数。当您使用MySQL或其他数据库服务时，为了确保通信的安全性，您可能会选择使用`SSL/TLS`加密连接。为了使`SSL/TLS`工作，您需要一个有效的证书。

MySQL参数变量auto_generate_certs用于控制MySQL是否会自动生成SSL/TLS证书以用于安全连接。如果这个变量设置为ON，MySQL将会生成SSL/TLS证书，而不需要使用外部证书。

要设置这个变量，首先可在MySQL服务器的my.cnf配置文件中添加如下的语句：

```sql
auto_generate_certs=ON
```

之后，需要重启MySQL服务以使变量生效。

## auto_increment_increment
>
>**ID自动递增增量**
create table test(id int auto_increment primary key, name varchar(32));

配合`auto_increment_offset` 一起使用

## auto_increment_offset

>**ID自动递增偏移**
>来源： <https://www.cnblogs.com/kerrycode/p/11150782.html>

- `auto_increment_offset`：AUTO_INCREMENT列值的起点，也就是初始值。取值范围是1 .. 65535
- `auto_increment_increment`：控制列中的值的增量值，也就是步长。其默认值是1，取值范围是1 .. 65535

**注意**：设置全局系统变量时，对当前连接或已存在的连接不生效，只对新的连接有效。

**注意**：如果设置负数，默认为1；如果设置超过65535的数，默认65535.

**注意**：如果表没有值，自增列第一个值为auto_increment_offset。

**注意**：如果auto_increment_offset的值大于auto_increment_increment的值，则auto_increment_offset的值会被忽略。

自增列的计算逻辑为 `auto_increment_offset + N × auto_increment_increment`  N表示第几次，从1开始计算（auto_increment_offset=1），并且计算值必须大于自增列的最大值（Max(ID)),

对于第一种情况： id  1、2，   因为最大值为2，而自增列的取值为1+1*3= 4， 所以自增列取值为4

对于第二种情况： id= 1、2、3. 因为最大值为3，而自增列的取值为1+1*3= 4， 所以自增列取值为4

auto_increment_offset修改后，自增列的变化规律
max(id)+(new_offset-old_offset)+increment ，也就是说变化auto_increment_offset后的第一个值为max(id)+(new_offset-old_offset)+increment之后再按步长递增。

## autocommit
>
>**自动提交**

- 手动提交：autocommit=0   / autocommit=OFF
当用户执行start transaction命令时（事务初始化），一个事务开启，当用户执行commit命令时当前事务提交。
从用户执行start transaction命令到用户执行commit命令之间的一系列操作为一个完整的事务周期。
若不执行commit命令，系统则默认事务回滚。

- 自动提交：autocommit=1   / autocommit=ON (系统默认值)
如果用户在当前情况下（参数autocommit=1）未执行start transaction命令而对数据库进行了操作，系统则默认用户对数据库的每一个操作为一个孤立的事务，
也就是说用户每进行一次操作系都会即时提交或者即时回滚。这种情况下用户的每一个操作都是一个完整的事务周期。

修改
使mysql中的autocommit 自动提交事务永久关闭，可修改mysql配置文件my.cnf，将autocommit=0或者autocommit=OFF添加：
[mysqld]
autocommit=OFF
或者
[mysqld]
autocommit=0
以上两者添加任意一个即可永久关闭mysql数据库默认的事务提交

然后使用重启命令：service mysqld restart重新启动mysql数据库服务，使用SHOW VARIABLES LIKE 'autocommit';查看autocommit状态即可永久关闭

## automatic_sp_privileges
>
>该参数控制着server是否自动分配execute和alter权限给创建routine的用户。 默认为1，自动赋权。

通常，数据库系统需要特定的权限以访问特定的存储过程，以便运行该存储过程，而MySQL提供了一种自动设置权限的功能，也就是automatic_sp_privileges变量。**其默认设置为ON，可以令系统自动为每个用户分配存储过程执行特权，以使用户能够访问和使用分配给它们的存储过程。** 在大多数情况下，这是可取的；但是，由于安全性方面的原因，某些系统可能需要仅允许特定用户访问特定的存储过程，这时可以将此变数设置为OFF来拒止自动授证。

设置automatic_sp_privileges变量的方法如下：

1）使用MySQL客户端登录数据库服务器。
2）使用SET语句进行设置：
SET GLOBAL automatic_sp_privileges=OFF|ON;
3）确认设置：
SELECT @@GLOBAL.automatic_sp_privileges;

## avoid_temporal_upgrade

再使用5.6.4以后的MySQL在执行alter table语句时，**如果发现了5.6.4版本以前的时间字段，如time,datetime,timestamp，会自动将其升级到当前的MySQL版本，而在升级期间，实际上是需要重建整个表**。
例如在alter table … add index时，MySQL发现了一个5.6.4以前的timestamp列，就会在执行alter table期间，将该列也一并升级至当前MySQL版本。而升级期间会重建表，所以使用show processlist会看到copy to tmp table的状态，而alter table的执行自然也就变成了堵塞DML，并且执行时间变长。
这种特性可以通过参数avoid_temporal_upgrade来控制，该参数默认关闭。通过开启该参数set global avoid_temporal_upgrade=on，则alter table执行期间不会执行时间列的更新操作。
**该参数引用至5.7.6，也从5.7.6开始废弃，未来版本可能将不会再有该参数。**

## back_log

当MySQL接到连接请求时，会花费一点时间来检查连接信息和为这个连接创建线程，在这个时间内，MySQL不会响应新的连接请求，而这段时间内不被响应的连接请求，会先被缓存起来。
那么能够缓存多少连接呢？由back_log控制。**默认值由公式决定：50 + (max_connections / 5)，但默认值不会超过900。**
与此同时，**back_log的设置不能超过操作系统内核的TCP/IP连接请求队列的限制**，例如Linux的net.core.somaxconn。

## basedir

MySQL 安装基目录的路径。

## big_tables

**如果启用，服务器会将所有临时表存储在磁盘上，而不是存储在内存中**。这可以防止大多数需要大型临时表的SELECT操作出现表tbl_name已满错误，但也会减慢内存表所能满足的查询速度。

新连接的默认值为OFF（使用内存中的临时表）。**通常情况下，不应该需要启用此变量，因为服务器能够通过为小型临时表使用内存并根据需要切换到基于磁盘的表来自动处理大型结果集。**

## bind_address

3306端口监听在127.0.0.1，只有本机客户端可以访问，其他服务器无法访问
3306端口如果监听在0.0.0.0上，如果没有端口限制，那么其他服务器则可以连接该服务器的该端口

MySQL服务器在单个网络套接字上侦听TCP/IP连接。这个套接字绑定到一个地址，但一个地址可以映射到多个网络接口。要指定地址，请在服务器启动时设置bind_address=addr，其中addr是IPv4或IPv6地址或主机名。如果addr是主机名，则服务器将名称解析为IP地址并绑定到该地址。如果主机名解析为多个IP地址，则服务器使用第一个IPv4地址（如果有），否则使用第一个IPv6地址。

服务器处理不同类型的地址如下：

- **如果地址为`*`**，则服务器接受所有服务器主机IPv4接口上的TCP/IP连接，如果服务器主机支持IPv6，则接受所有IPv6接口上的TCP/IP连接。使用此地址可以**允许在所有服务器接口上进行IPv4和IPv6连接。此值为默认值。**

- **如果地址为`0.0.0.0`**，则服务器接受所有服务器主机IPv4接口上的TCP/IP连接。

- **如果地址为`::`**，则服务器接受所有服务器主机IPv4和IPv6接口上的TCP/IP连接。

- **如果该地址是IPv4映射的地址**，则服务器接受该地址的IPv4或IPv6格式的TCP/IP连接。例如，如果服务器绑定到`::ffff:127.0.0.1`，客户端可以使用`--host=127.0.0.1`或`--host=::ffff:127.0.0.1`进行连接。

- **如果地址是“常规”IPv4或IPv6地址（如127.0.0.1或::1）**，则服务器仅接受该IPv4或IPv6的TCP/IP连接。

如果绑定到地址失败，服务器将产生错误，并且不会启动。

如果您打算将服务器绑定到特定地址，请确保mysql.user系统表包含一个具有管理权限的帐户，您可以使用该帐户连接到该地址。否则，无法关闭服务器。例如，**如果将服务器绑定到`*`，则可以使用所有现有帐户连接到它**。但是，**如果将服务器绑定到::1，它只接受该地址上的连接。在这种情况下，首先确保"root"@"::1"帐户存在于mysql.user表中，这样您仍然可以连接到服务器以关闭它。**

此变量对嵌入式服务器（libmysqld）没有影响，并且在嵌入式服务器中不可见。

## binlog_cache_size
>
> 参考 <https://blog.51cto.com/u_13482808/7327078>
>
## binlog_checksum

## binlog_direct_non_transactional_updates

## binlog_error_action

## binlog_format

## binlog_group_commit_sync_delay

## binlog_group_commit_sync_no_delay_count

## binlog_gtid_simple_recovery

## binlog_max_flush_queue_time

## binlog_order_commits

## binlog_row_image

## binlog_rows_query_log_events

## binlog_stmt_cache_size

## binlog_transaction_dependency_history_size

## binlog_transaction_dependency_tracking

## block_encryption_mode

> 块加密模式

此变量控制诸如AES之类的基于块的算法的块加密模式。它会影响AES_ENCRYPT（）和AES_DECRYPT的加密。

block_encryption_mode采用aes keylen模式格式的值，其中keylen是以位为单位的密钥长度，mode是加密模式。该值不区分大小写。允许的keylen值为128、192和256。允许的加密模式取决于MySQL是使用OpenSSL还是yaSSL编译的：

- 对于OpenSSL，允许的模式值为：ECB、CBC、CFB1、CFB8、CFB128、OFB
- 对于yaSSL，允许的模式值为：ECB、CBC
  
  例如，此语句使AES加密函数使用256位的密钥长度和CBC模式：

  ```sql
  SET block_encryption_mode = 'aes-256-cbc';
  ```

尝试将block_encryption\umode设置为包含不支持的密钥长度的值或SSL库不支持的模式时出错。

## bulk_insert_buffer_size

> 大容量插入缓冲区大小
> 这个参数只能对 MyISAM使用，innodb无效

MyISAM 使用一种特殊的树状缓存来使批量插入更快。`INSERT ... SELECT`，`INSERT ... VALUES (...), (...)`, 在向非空表添加数据时使用`LOAD DATA`命令。。此变量限制缓存树的大小（以每个线程的字节为单位）。将其设置为0将禁用此优化。**默认值为8MB。**

## character_set_client

字符集客户端
System Variable系统变量 |character_set_client
--|--
Scope范围 |Global, Session全局，会话
Dynamic动态 |Yes
Type类型 |String
Default Value默认值

> utf8

从客户端到达的语句的字符集。此变量的会话值是使用客户端连接到服务器时客户端请求的字符集设置的。（许多客户端支持--default字符集选项，以便显式指定此字符集。另请参阅第10.4节“连接字符集和排序规则”。）当客户端请求的值未知或不可用，或者服务器配置为忽略客户端请求时，变量的全局值用于设置会话值：

- 客户端请求服务器未知的字符集。例如，启用日语的客户端在连接到未配置sjis支持的服务器时请求sjis。
- 客户端来自MySQL 4.1之前的MySQL版本，因此不请求字符集。
- mysqld是从--skip字符集客户端握手选项开始的，这会导致它忽略客户端字符集配置。这再现了MySQL 4.0的行为，如果您希望在不升级所有客户端的情况下升级服务器，这将非常有用。
  
某些字符集不能用作客户端字符集。试图将它们用作character_set_client值会产生错误。请参见不允许的客户端字符集。

- ucs2
- utf16
- utf16le
- utf32

## character_set_connection

> 字符集连接
主要用来设置连接数据库时的字符集，如果程序中没有指明连接数据库使用的字符集类型则按照这个字符集设置。

## character_set_database

**此选项是动态的，但应仅由服务器设置。不应手动设置此变量。**

默认数据库使用的字符集。每当默认数据库发生更改时，服务器都会设置此变量。如果没有默认数据库，则变量的值与character_set_server的值相同。

MySQL 5.7中不推荐使用全局`character_set_database`和`collating_database`系统变量；期望它们在MySQL的未来版本中被删除。

在MySQL 5.7中，不赞成为会话`character_set_database`和`collating_database`系统变量赋值，赋值会产生警告。您应该期望会话变量在MySQL的未来版本中变为只读，并且赋值会产生错误，同时仍然可以访问会话变量来确定默认数据库的数据库字符集和排序规则。

## character_set_filesystem

文件系统的编码格式，把操作系统上的文件名转化成此字符集，即把 character_set_client转换character_set_filesystem， 默认binary是不做任何转换的。

文件系统字符集。此变量用于解释引用文件名的字符串文字，例如`LOAD DATA`和`SELECT。。。INTO OUTFILE`语句和`LOAD_FILE()`函数。在尝试打开文件之前，这些文件名会从`character_set_client`转换为`character_set_filesystem`。默认值为二进制，这意味着不会发生转换。对于允许使用多字节文件名的系统，可能更适合使用不同的值。
例如，如果系统使用UTF-8表示文件名，请将`character_set_filesystem设置为'utf8mb4'`。

## character_set_results

数据库给客户端返回时使用的编码格式，如果没有指明，使用服务器默认的编码格式。
用于向客户端返回查询结果的字符集。这包括结果数据（如列值）、结果元数据（如列名）和错误消息。

## character_set_server

服务器安装时指定的默认编码格式，这个变量建议由系统自己管理，不要人为定义。
服务器的默认字符集。如果设置了此变量，还应该设置collification_server来指定字符集的排序规则。

latin1,Latin1是ISO-8859-1的别名,有些环境下写作Latin-1。

## character_set_system

数据库系统使用的编码格式，这个值一直是utf8，不需要设置，它是为存储系统元数据的编码格式。

## character_sets_dir

这个变量是字符集安装的目录。

## check_proxy_users
>
>检查代理用户
>

一些身份验证插件为自己实现代理用户映射（例如PAM和Windows身份验证插件）。默认情况下，其他身份验证插件不支持代理用户。其中，有些人可以请求MySQL服务器本身根据授予的代理权限映射代理用户：MySQL_native_password、sha256_password。

如果启用了check_proxy_users系统变量，则服务器将为发出此类请求的任何身份验证插件执行代理用户映射。然而，也可能需要启用特定于插件的系统变量，以利用服务器代理用户映射支持：

- 对于mysql_native_password插件，请启用mysql_native/password_proxy_users。
- 对于sha256_password插件，请启用sha256_pass word_proxy_users。

## collation_connection
>
>排序规则连接

连接字符集的排序规则。colloration_connection对于文字字符串的比较非常重要。对于字符串与列值的比较，排序规则连接无关紧要，因为列有自己的排序规则，排序规则优先级更高（请参阅第10.8.4节“表达式中的排序规则强制性”）。

## collation_database
>
>排序规则数据库
>此选项是动态的，但应仅由服务器设置。不应手动设置此变量。

默认数据库使用的排序规则。每当默认数据库发生更改时，服务器都会设置此变量。如果没有默认数据库，则该变量的值与排序规则服务器的值相同。

MySQL 5.7中不推荐使用全局character_set_database和collating_database系统变量；期望它们在MySQL的未来版本中被删除。

## collation_server
>
>排序规则服务器

服务器的默认排序规则。

## completion_type  
>
>完成类型

事务处理完成类型。此变量可以采用下表中所示的值。可以使用名称值或相应的整数值来分配变量。
Value|Description
--|--
NO_CHAIN (or 0)|COMMIT和ROLLBACK不受影响。这是默认值。
CHAIN (or 1)|COMMIT和ROLLBACK分别等效于COMMIT and CHAIN和ROLLBACK and CHAIN。（新事务立即开始，隔离级别与刚刚终止的事务相同。）
RELEASE (or 2)|COMMIT和ROLLBACK分别等效于COMMIT RELEASE和ROLLBACK RELEASE。（服务器在终止事务后断开连接。）

completion_type影响以START TRANSACTION或begin开头、以COMMIT或ROLLBACK结尾的事务。它不适用于因执行第13.3.3节“导致隐式提交的语句”中列出的语句而产生的隐式提交。它也不适用于XA COMMIT、XA ROLLBACK或当autocommit=1时。

## concurrent_insert
>
>并行插入

如果为AUTO（默认值），MySQL将允许INSERT和SELECT语句同时运行，用于在数据文件中间没有空闲块的MyISAM表。

此变量可以采用下表中所示的值。可以使用名称值或相应的整数值来分配变量。

Value|Description
--|--
NEVER (or 0)|禁用并发插入
AUTO (or 1)|（默认设置）为没有孔的MyISAM表启用并发插入
ALWAYS (or 2)|为所有MyISAM表（即使是那些有孔的表）启用并发插入。对于带有孔的表，如果另一个线程正在使用它，则会在表的末尾插入新行。否则，MySQL将获得一个普通的写锁，并将行插入孔中。

 如果您使用--skip-new启动mysqld，那么concurrent_insert将设置为NEVER。

## connect_timeout  
>
>连接超时

mysqld服务器在使用Bad握手进行响应之前等待连接数据包的秒数。默认值为10秒。

如果客户端经常遇到以下错误，增加connect_timeout值可能会有所帮助：
`Lost connection to MySQL server at 'XXX', system error: errno.`
与位于“XXX”的MySQL服务器的连接丢失，系统错误：errno。

## core_file
>
>核心文件

MySQL服务器数据目录的路径。相对路径是相对于当前目录解析的。如果您希望服务器自动启动（也就是说，在无法假设当前目录是什么的上下文中），最好将datadir值指定为绝对路径。

## datadir
>
>数据目录
>
## date_format
>
>日期格式

此变量未使用。它已被弃用，并在MySQL 8.0中被删除。

## datetime_format
>
>日期时间格式

此变量未使用。它已被弃用，并在MySQL 8.0中被删除。

## default_authentication_plugin
>
>默认身份验证插件

默认的身份验证插件。这些值是允许的：

- mysql_native_password：使用mysql本机密码(默认值)
- sha256_password：使用SHA-256密码

如果此变量的值不是mysql_native_password，则mysql 5.5.7之前的客户端将无法连接，因为在允许的默认身份验证插件中，它们只了解mysql_native_password身份验证协议。

default_authentication_plugin值会影响服务器操作的以下方面：

- 它确定服务器将哪个身份验证插件分配给CREATE USER和GRANT语句创建的新帐户，这些语句没有明确指定身份验证插件。
- old_passwords系统变量会影响使用mysql_native_password或sha256_password身份验证插件的帐户的密码哈希。如果默认的身份验证插件是其中一个插件，则服务器会在启动时将old_passwords设置为插件密码哈希方法所需的值。
- 对于使用以下任一语句创建的帐户，服务器会将该帐户与默认的身份验证插件相关联，并根据该插件的要求为该帐户分配给定的密码：

    ```sql
    CREATE USER ... IDENTIFIED BY 'cleartext password';
    GRANT ...  IDENTIFIED BY 'cleartext password';
    ```

- 对于使用以下任一语句创建的帐户，如果密码哈希具有插件所需的格式，则服务器会将该帐户与默认身份验证插件相关联，并为该帐户分配给定的密码哈希：

    ```sql
    CREATE USER ... IDENTIFIED BY PASSWORD 'encrypted password';
    GRANT ...  IDENTIFIED BY PASSWORD 'encrypted password';
    ```

如果密码哈希不是默认身份验证插件所需的格式，则该语句将失败。

## default_password_lifetime
>
>默认密码生存期

此变量定义全局自动密码过期策略。默认的default_password_lifetime值为0，这将禁用密码自动过期。如果default_password_lifetime的值是正整数N，则表示允许的密码生存期；密码必须每N天更改一次。

**note**
在MySQL 5.7.11之前，默认的default_password_lifetime值为360（密码必须大约每年更改一次）。对于这些版本，请注意，如果不对default_password_lifetime变量或单个用户帐户进行更改，则所有用户密码将在360天后过期，并且当发生这种情况时，所有用户帐户都将开始以受限模式运行。连接到服务器的客户端（实际上是用户）随后收到一个错误，指示必须更改密码：错误1820（HY000）：在执行此语句之前，必须使用ALTER USER语句重置密码。  

但是，对于自动连接到服务器的客户端（例如通过脚本进行的连接）来说，这很容易错过。为了避免这些客户端由于密码过期而突然停止工作，请确保更改这些客户端的密码过期设置，如下所示：

```sql
ALTER USER 'script'@'localhost' PASSWORD EXPIRE NEVER;
```

或者，将default_password_lifetime变量设置为0，从而禁用所有用户的密码自动过期。

## default_storage_engine
>
>默认存储引擎

要查看哪些存储引擎可用并已启用，请使用SHOW engines语句或查询INFORMATION_SCHEMA engines表。

如果在服务器启动时禁用默认存储引擎，则必须将永久表和临时表的默认引擎设置为其他引擎，否则服务器将无法启动。

## default_tmp_storage_engine
>
>默认tmp存储引擎

临时表的默认存储引擎（使用CREATE TEMPORARY TABLE创建）。要为永久表设置存储引擎，请设置default_storage_engine系统变量。另请参阅关于该变量可能值的讨论。

如果在服务器启动时禁用默认存储引擎，则必须将永久表和临时表的默认引擎设置为其他引擎，否则服务器将无法启动。

## default_week_format
>
>默认周格式

用于`WEEK()`函数的默认模式值。

## delay_key_write
>
>延迟键写入

此变量指定如何使用延迟的密钥写入。它**仅适用于MyISAM表**。延迟的密钥写入会导致在写入之间不刷新密钥缓冲区。另请参见第15.2.1节“MyISAM启动选项”。

此变量可以具有以下值之一，以影响可在CREATE table语句中使用的DELAY_KEY_WRITE表选项的处理。

Option|Description
--|--
OFF|DELAY_KEY_WRITE被忽略。
ON|MySQL支持CREATE TABLE语句中指定的任何DELAY_KEY_WRITE选项。这是默认值。
ALL|所有新打开的表都被视为是在启用DELAY_KEY_WRITE选项的情况下创建的。

如果将此变量设置为ALL，则在使用其他程序（如其他MySQL服务器或myisamchk）中的MyISAM表时，不应使用这些表。这样做会导致索引损坏。

如果为表启用了DELAY_KEY_WRITE，则不会在每次索引更新时为表刷新键缓冲区，而是仅在表关闭时才刷新。这大大加快了对键的写入速度，但如果使用此功能，则应通过使用MyISAM_recover_options系统变量集（例如，MyISAM_recover_options='BACKUP，FORCE'）启动服务器来添加对所有MyISAM表的自动检查。请参阅第5.1.7节“服务器系统变量”和第15.2.1节“MyISAM启动选项”。

如果使用`--skip-new`启动mysqld，delay_key_write将设置为OFF。

## delayed_insert_limit
>
>延迟插入限制

不赞成使用此系统变量（因为不支持DELAYED插入）；预计它将在未来的版本中删除。

## delayed_insert_timeout
>
>延迟插入超时

不赞成使用此系统变量（因为不支持DELAYED插入）；预计它将在未来的版本中删除。

## delayed_queue_size
>
>延迟队列大小

不赞成使用此系统变量（因为不支持DELAYED插入）；预计它将在未来的版本中删除。

## disabled_storage_engines
>
>禁用的存储引擎

此变量指示哪些存储引擎不能用于创建表或表空间。例如，为了防止创建新的MyISAM或FEDERATED表，请在服务器选项文件中使用以下行启动服务器：

```sql
[mysqld]
disabled_storage_engines="MyISAM,FEDERATED"
```

默认情况下，disabled_storage_engines为空（没有禁用任何引擎），但可以将其设置为一个或多个引擎的逗号分隔列表（不区分大小写）。值中命名的任何引擎都不能用于使用`create TABLE`或`create TABLESPACE`创建表或表空间，也不能与`ALTER TABLE...ENGINE`或`ALTER TABLESPACE...ENGINE`一起使用。更改现有表或表空间的存储引擎。尝试执行此操作会导致`ER_DISABLED_STORAGE_ENGINE`错误。

`disabled_storage_engines`不限制现有表的其他DDL语句，如`CREATE INDEX、TRUNCATE TABLE、ANALYZE TABLE、DROP TABLE或DROP TABLESPACE`。这允许平滑转换，以便使用禁用引擎的现有表或表空间可以通过`ALTER TABLE...ENGINE permitted_engine.`…等方式迁移到允许的引擎。

允许将`default_storage_engine`或`default_tmp_storage_engine`系统变量设置为禁用的存储引擎。这可能会导致应用程序行为不稳定或失败，尽管这在开发环境中可能是一种有用的技术，用于识别使用禁用引擎的应用程序，以便对其进行修改。

disabled_storage_engines将被禁用，如果服务器是使用以下任何选项启动的，则它将无效：`--bootstrap、--initialize、--initiate unsecurity和--skip grant tables。`

设置`disabled_storage_engines`可能会导致`mysql_upgrade`出现问题。有关详细信息，请参见第4.4.7节“mysql_upgrade--检查和升级mysql表”。

## disconnect_on_expired_password
>
>密码过期时断开连接

此变量控制服务器如何处理密码过期的客户端：

- 如果客户端表示可以处理过期密码，则disconnect_on_expired_password的值无关紧要。服务器允许客户端进行连接，但将其置于沙箱模式。
- 如果客户端没有指示可以处理过期密码，则服务器将根据disconnect_on_expired_password的值来处理客户端：
  - 如果已启用disconnect_on_expired_password:，则服务器将断开客户端的连接。
  - 如果disconnect_on_expired_password:被禁用，则服务器允许客户端进行连接，但将其置于沙箱模式。

有关与过期密码处理相关的客户端和服务器设置交互的更多信息，请参阅第6.2.12节“过期密码的服务器处理”。

## div_precision_increment
>
>div精度增量

此变量表示用/运算符执行的除法运算的结果的位数。默认值为4。最小值和最大值分别为0和30。以下示例说明了增加默认值的效果。

```sql
mysql> SELECT 1/7;
+--------+


> 1/7    |
+--------+


> 0.1429 |
+--------+
mysql> SET div_precision_increment = 12;
mysql> SELECT 1/7;
+----------------+


> 1/7            |
+----------------+


> 0.142857142857 |
+----------------+
```

## end_markers_in_json
>
>json中的结束标记

优化器JSON输出是否应添加结束标记。请参阅MySQL内部：end_markers_in_json系统变量。

## enforce_gtid_consistency
>
>强制gtid一致性

主从数据库相关

## eq_range_index_dive_limit
>
>eq范围指数下降极限

当优化器在估计符合条件的行数时应从使用索引潜水切换到使用索引统计信息时，此变量指示相等比较条件中相等范围的数量。它适用于具有以下等效形式之一的表达式的求值，其中优化器使用非唯一索引来查找col_name值：

```sql
col_name IN(val1, ..., valN)
col_name = val1 OR ... OR col_name = valN
```

在这两种情况下，表达式都包含N个相等范围。优化器可以使用索引潜水或索引统计信息进行行估计。如果eq_range_index_dive_limit大于0，则如果存在eq_range_index_dive-limit或更多相等范围，则优化器将使用现有的索引统计信息，而不是索引潜水。因此，要允许对多达N个相等范围使用索引潜水，请将eq_range_index_dive_limit设置为N+1。要禁用索引统计信息的使用并始终使用索引潜水（无论N），请将eq_range_index_dive_limit设置为0。

## error_count
>
>错误计数

生成消息的最后一条语句所导致的错误数。此变量是只读的。参见第13.7.7.17节“显示错误声明”。

## event_scheduler
>
>事件调度程序

此变量启用或禁用以及启动或停止事件计划程序。可能的状态值为ON、OFF和DISABLED。关闭事件计划程序与禁用事件计划程序不同，后者需要将状态设置为DISABLED。在第23.4.2节“事件调度器配置”中更详细地讨论了此变量及其对事件调度器操作的影响

## expire_logs_days
>
>过期日志天数
>
## explicit_defaults_for_timestamp
>
>时间戳的显式默认值

此系统变量确定服务器是否为TIMESTAMP列中的默认值和NULL值处理启用某些非标准行为。默认情况下，explicit_defaults_for_timestamp处于禁用状态，从而启用非标准行为。

如果explicit_defaults_for_timestamp被禁用，则服务器将启用非标准行为并按如下方式处理timestamp列：

- 未使用NULL属性显式声明的TIMESTAMP列将自动使用not NULL属性声明。允许为此类列指定NULL值，并将该列设置为当前时间戳。
- 如果表中的第一个TIMESTAMP列没有显式声明为NULL属性或显式DEFAULT或ON UPDATE属性，则会自动声明为DEFAULT CURRENT_TIMESTAMP和ON UPDATE CURRENT_IMESTAMP属性。
- 如果没有用NULL属性或显式DEFAULT属性显式声明第一个列之后的TIMESTAMP列，则会自动声明为DEFAULT“0000-00-00 00:00:00”（“零”时间戳）。对于未为此类列指定显式值的插入行，将为该列分配“0000-00-00 00:00:00”，并且不会出现任何警告。
- 根据启用的是严格SQL模式还是NO_ZERO_DATE SQL模式，默认值“0000-00-00 00:00:00”可能无效。请注意，传统SQL模式包括严格模式和NO_ZERO_DATE。请参阅第5.1.10节“服务器SQL模式”。

不赞成使用刚才描述的不规范行为；期望它们在MySQL的未来版本中被删除。

如果启用了explicit_defaults_for_timestamp，则服务器将禁用非标准行为，并按如下方式处理timestamp列：

- 不能为TIMESTAMP列分配NULL值以将其设置为当前时间戳。要分配当前时间戳，请将该列设置为current_timestamp或类似NOW（）的同义词。
- 没有用not NULL属性显式声明的TIMESTAMP列会自动用NULL属性声明，并允许NULL值。为此类列指定NULL值会将其设置为NULL，而不是当前时间戳。
- 使用NOT NULL属性声明的TIMESTAMP列不允许NULL值。对于为此类列指定NULL的插入，如果启用了严格SQL模式，则结果为单行插入错误，或者如果禁用了严格SQL方式，则为多行插入插入“0000-00-00 00:00:00”。在任何情况下，为列分配NULL值都不会将其设置为当前时间戳。
- 没有使用DEFAULT CURRENT_TIMESTAMP或ON UPDATE CURRENT_IMESTAMP属性自动声明TIMESTAMP列。必须明确指定这些属性。
- 表中的第一列TIMESTAMP与第一列之后的TIMESTAMP列没有不同的处理方式。

如果在服务器启动时禁用explicit_defaults_for_timestamp，则错误日志中会出现此警告：

```sql
[Warning] TIMESTAMP with implicit DEFAULT value is deprecated.
Please use --explicit_defaults_for_timestamp server option (see
documentation for more details).
```

如警告所示，要禁用不推荐使用的非标准行为，请在服务器启动时启用explicit_defaults_for_timestamp系统变量。

> explicit_defaults_for_timestamp本身是不赞成使用的，因为它的唯一目的是允许控制不赞成使用timestamp的行为，这些行为将在MySQL的未来版本中删除。当删除这些行为时，explicit_defaults_for_timestamp不再有任何用途，您也可以期待它被删除。

## external_user
>
>外部用户

身份验证过程中使用的外部用户名，由用于验证客户端的插件设置。使用本机（内置）MySQL身份验证，或者如果插件没有设置值，则此变量为NULL。参见第6.2.14节“代理用户”。

## flush
>
>脸红

如果为ON，则服务器会在每次SQL语句之后将所有更改刷新（同步）到磁盘。通常，MySQL只在每条SQL语句之后将所有更改写入磁盘，并让操作系统处理与磁盘的同步。请参阅B.3.3.3节“如果MySQL持续崩溃该怎么办”。如果使用--flush选项启动mysqld，则此变量设置为ON。

> 如果启用了flush，flush_time的值无关紧要，对flush_time的更改对flush行为没有影响。

## flush_time
>
>冲洗时间

如果设置为非零值，则每隔flush_time秒关闭所有表，以释放资源并将未刷新的数据同步到磁盘。此选项最好仅在资源最少的系统上使用。

> 如果启用了flush，flush_time的值无关紧要，对flush_time的更改对flush行为没有影响。

## foreign_key_checks
>
>外键检查

如果设置为1（默认值），则会检查外键约束。如果设置为0，则忽略外键约束，但有几个例外。重新创建已删除的表时，如果表定义不符合引用该表的外键约束，则会返回错误。同样，如果外键定义的格式不正确，ALTER TABLE操作也会返回错误。有关更多信息，请参阅第13.1.18.5节“FOREIGN KEY约束”。

设置此变量对NDB表的效果与对InnoDB表的效果相同。通常，在正常操作期间启用此设置，以强制执行引用完整性。禁用外键检查对于以不同于父/子关系所需的顺序重新加载InnoDB表非常有用。参见第13.1.18.5节“外国密钥约束”。

将foreign_key_checks设置为0也会影响数据定义语句：DROP SCHEMA将删除架构，即使该架构包含具有由架构外的表引用的外键的表也是如此；DROP TABLE将删除具有由其他表引用的主键的表。

> 将foreign_key_checks设置为1不会触发对现有表数据的扫描。因此，foreign_key_checks=0时添加到表中的行不会验证一致性。
> 即使foreign_key_checks=0，也不允许删除外键约束所需的索引。在删除索引之前，必须删除外键约束（Bug#70260）。
>
## ft_boolean_syntax
>
>ft布尔语法

使用IN boolean MODE执行的布尔全文搜索支持的运算符列表。参见第12.9.2节“布尔全文搜索”。

默认变量值为`+ -><()~*:""&|`。更改值的规则如下：

- 运算符函数由字符串中的位置决定。
- 替换值必须为14个字符。
- 每个字符都必须是ASCII非字母字符。
- 第一个或第二个字符必须是空格。
- 除了位置11和12的短语引用运算符外，不允许重复。这两个字符不需要相同，但它们是唯一可能相同的两个字符。
- 位置10、13和14（默认情况下设置为：、&和|）保留用于将来的扩展。

## ft_max_word_len
>
>ft最大字长度 10~84

MyISAM FULLTEXT索引中要包含的单词的最大长度。

> 更改此变量后，必须重新生成MyISAM表上的FULLTEXT索引。使用 `REPAIR TABLE tbl_name QUICK`.

## ft_min_word_len
>
>ft最小单词len

要包含在MyISAM FULLTEXT索引中的单词的最小长度。

> 更改此变量后，必须重新生成MyISAM表上的FULLTEXT索引。使用 `REPAIR TABLE tbl_name QUICK`.

## ft_query_expansion_limit
>
>ft查询扩展限制

要用于使用WITH QUERY EXPANSION执行全文搜索的前匹配项数。

## ft_stopword_file
>
>ft停止字文件

从中读取MyISAM表全文搜索的停止词列表的文件。服务器会在数据目录中查找文件，除非提供了一个绝对路径名来指定不同的目录。文件中的所有单词都已使用；评论不受尊重。默认情况下，会使用内置的停止语列表（如存储/myisam/ft_static.c文件中所定义的）。将此变量设置为空字符串（“”）将禁用停止字筛选。另见第12.9.4节“全文停止语”。

> 更改此变量或停止字文件的内容后，必须重新生成MyISAM表上的FULLTEXT索引。快速使用维修表tbl_name。
>
## general_log
>
>常规日志

是否启用了常规查询日志。该值可以为0（或OFF）以禁用日志，也可以为1（或ON）以启用日志。日志输出的目的地由log_output系统变量控制；如果该值为NONE，则即使启用了日志，也不会写入任何日志条目。

## general_log_file
>
>常规日志文件

常规查询日志文件的名称。默认值为host_name.log，但可以使用--general_log_file选项更改初始值。

## group_concat_max_len
>
>组concat最大len

GROUP_CONCT（）函数允许的最大结果长度（以字节为单位）。默认值为1024。

## gtid_executed_compression_period
>
> gtid执行的压缩周期

如果zlib压缩库可用于服务器，则为YES；如果不可用，则为NO。否则，COMPRESS（）和UNCOMPRESS（）函数将无法使用。

## gtid_mode
>
> gtid模式

集群

## gtid_next
>
> gtid下一个

## gtid_owned
>
> gtid拥有

## gtid_purged
>
> gtid已清除

## have_compress
>
> 有压缩

## have_crypt
>
> 有crypt

如果crypt（）系统调用可用于服务器，则为YES；如果不可用，则为NO。如果没有，则无法使用ENCRYPT（）函数。

ENCRYPT（）函数在MySQL 5.7中已弃用，将在将来的MySQL版本中删除，并且不应再使用。（对于单向哈希，请考虑使用SHA2（）。）因此，have_crypt也被弃用；预计它将在未来的版本中删除。

## have_dynamic_loading
>
> 具有动态负载

如果mysqld支持动态加载插件，则为YES；如果不支持，则为NO。如果值为NO，则不能使用诸如--plugin-load之类的选项在服务器启动时加载插件，也不能使用INSTALL plugin语句在运行时加载插件。

## have_geometry
>
> 具有几何图形

是（如果服务器支持空间数据类型），否（如果不支持）。

## have_openssl
>
> 具有openssl

此变量是have_ssl的同义词。

## have_profiling
>
> 具有配置文件

如果存在语句分析功能，则为YES；如果不存在，则为NO。如果存在，配置文件系统变量控制是启用还是禁用此功能。参见第13.7.5.31节“SHOW PROFILES声明”。

**此变量已弃用；期望它在MySQL的未来版本中被删除。**

## have_query_cache
>
> 具有查询缓存

如果mysqld支持查询缓存，则为YES；如果不支持，则为NO。

**从MySQL 5.7.20开始，查询缓存已被弃用，并在MySQL 8.0中被删除。弃用包括have_query_cache。
**

## have_rtree_keys

> 有rtree密钥

是（如果RTREE索引可用），否（如果不可用）。（这些用于MyISAM表中的空间索引。）

## have_ssl
>
> 具有ssl

如果mysqld支持SSL连接，则为YES；如果服务器是使用SSL支持编译的，但没有使用适当的连接加密选项启动，则为DISABLED。有关更多信息，请参阅第2.8.6节“配置SSL库支持”。

## have_statement_timeout
>
> 有语句超时

语句执行超时功能是否可用（请参阅语句执行时间优化器提示）。如果此功能使用的后台线程无法初始化，则该值可以为NO。

## have_symlink
>
> 具有符号链接

如果启用了符号链接支持，则为YES；如果未启用，则为NO。这是Unix上支持DATA DIRECTORY和INDEX DIRECTORY表选项所必需的。如果服务器是使用--skip符号链接选项启动的，则该值为DISABLED。

**此变量在Windows上没有任何意义。**

## host_cache_size
>
> 主机缓存大小

MySQL服务器维护一个内存中的主机缓存，该缓存包含客户端主机名和IP地址信息，用于避免域名系统（DNS）查找；请参阅第5.1.1.2节“DNS查找和主机缓存”。

host_cache_size变量控制主机缓存的大小，以及公开缓存内容的性能架构host_cache表的大小。设置host_cache_size具有以下效果：

- 将大小设置为0将禁用主机缓存。在禁用缓存的情况下，服务器每次连接客户端时都会执行DNS查找。
- 在运行时更改大小会导致隐式主机缓存刷新操作，该操作会清除主机缓存、截断host_cache表并取消阻止任何被阻止的主机。

默认值自动设置为128，最大连接数不超过500时加1，最大连接值超过500时每增加20加1，上限为2000。

使用--skip-host-cache选项类似于将host_cache_size系统变量设置为0，但host_cache_size更灵活，因为它还可以用于在运行时调整主机缓存的大小、启用和禁用主机缓存，而不仅仅是在服务器启动时。

使用--skip主机缓存启动服务器不会阻止运行时更改host_cache_size的值，但这些更改没有任何效果，并且即使host_cache_size设置为大于0，也不会重新启用缓存。

出于上一段中给出的原因，首选设置host_cache_size系统变量，而不是--skip-host-cache选项。此外，**--skip-host-cache选项在MySQL 8.0中已被弃用，预计在未来版本的MySQL中将删除该选项。**

## hostname
>
> 主机名

服务器在启动时将此变量设置为服务器主机名。

## identity
>
> 身份

此变量是last_insert_id变量的同义词。它的存在是为了与其他数据库系统兼容。您可以使用SELECT@@identity读取其值，并使用set identity设置它。

## ignore_builtin_innodb
>
> 忽略内置的innodb

## ignore_db_dirs
>
> 忽略数据库目录

数据目录中不被视为数据库目录的名称的逗号分隔列表。该值是从服务器启动时给定的--ignore db dir的任何实例中设置的。

从MySQL 5.7.11开始，--ignore db dir可以在数据目录初始化时与mysqld一起使用--initialize来指定服务器应该忽略的目录，以评估现有数据目录是否为空。见2.9.1节“初始化数据目录”。

MySQL 5.7中不赞成使用此系统变量。随着MySQL 8.0中数据字典的引入，它变得多余，并在该版本中被删除。

## init_connect
>
> 初始化连接

由服务器为每个连接的客户端执行的字符串。该字符串由一个或多个SQL语句组成，用分号分隔。

对于具有SUPER权限的用户，不会执行init_connect的内容。这样做是为了使init_connect的错误值不会阻止所有客户端进行连接。例如，该值可能包含一个语法错误的语句，从而导致客户端连接失败。不为具有SUPER权限的用户执行init_connect使他们能够打开连接并修复init_conneck值。

从MySQL 5.7.22开始，任何密码过期的客户端用户都会跳过init_connect执行。这样做是因为这样的用户无法执行任意语句，因此init_connect执行失败，导致客户端无法连接。通过跳过init_connect执行，用户可以连接并更改密码。

服务器将丢弃init_connect值中的语句生成的任何结果集。

## init_file
>
> init文件

如果指定，此变量将命名一个文件，该文件包含要在启动过程中读取和执行的SQL语句。每条语句必须在一行上，并且不应包含注释。

如果服务器是使用任何--bootstrap、--initialize或--initialized不安全选项启动的，则它将在bootstap模式下运行，并且某些功能不可用，从而限制了文件中允许的语句。其中包括与帐户管理（如CREATE USER或GRANT）、复制和全局事务标识符相关的语句。请参阅第16.1.3节“使用全局事务标识符进行复制”。

## init_slave
>
> 初始化slave

## innodb_xxx

InnoDB系统变量列在第14.15节“InnoDB启动选项和系统变量”中。这些变量控制着InnoDB表的存储、内存使用和I/O模式的许多方面，在InnoDB是默认存储引擎的情况下，这些变量尤为重要。

<https://dev.mysql.com/doc/refman/5.7/en/innodb-parameters.html>

## insert_id
>
> 插入id

插入AUTO_INCREMENT值时，以下INSERT或ALTER TABLE语句要使用的值。这主要用于二进制日志。

## interactive_timeout
>
> 交互式超时

服务器在关闭交互式连接之前等待活动的秒数。交互式客户端定义为对mysql_real_connect（）使用client_interactive选项的客户端。另请参见wait_timeout。

## internal_tmp_disk_storage_engine

> 内部tmp磁盘存储引擎

磁盘上内部临时表的存储引擎（请参阅第8.4.4节“MySQL中的内部临时表使用”）。允许的值为MYISAM和INNODB（默认值）。

优化器使用internal_tmp_disk_storage_engine为磁盘上的内部临时表定义的存储引擎。

当使用internal_tmp_disk_storage_engine=INNODB（默认值）时，在磁盘上生成超过INNODB行或列限制的内部临时表的查询会返回row size too large或too many columns error。解决方法是将internal_tmp_disk_storage_engine设置为MYISAM。

## join_buffer_size

> 联接缓冲区大小

用于纯索引扫描、范围索引扫描以及不使用索引并因此执行全表扫描的联接的缓冲区的最小大小。通常，获得快速联接的最佳方法是添加索引。当无法添加索引时，增加join_buffer_size的值以获得更快的完全联接。为两个表之间的每个完整联接分配一个联接缓冲区。对于不使用索引的多个表之间的复杂联接，可能需要多个联接缓冲区。

默认值为256KB。join_buffer_size的最大允许设置为4GB−1。64位平台允许使用更大的值（64位Windows除外，对于64位Windows，较大的值会截断为4GB−1并发出警告）。块大小为128，在存储系统变量的值之前，MySQL Server会将不是块大小的精确倍数的值四舍五入到块大小的下一个较低倍数。解析器允许平台的最大无符号整数值（对于32位系统为4294967295或232−1，对于64位系统为18446744073709551615或264−1），但实际最大值要低一个块大小。

除非使用块嵌套循环或批处理密钥访问算法，否则将缓冲区设置为大于容纳每个匹配行所需的缓冲区不会带来任何好处，并且所有联接都至少分配最小大小，因此在全局范围内将此变量设置为大值时要小心。最好保持全局设置较小，并仅在执行大型联接的会话中将会话设置更改为较大值。如果全局大小大于大多数使用内存分配时间的查询所需的大小，那么内存分配时间可能会导致性能大幅下降。

当使用块嵌套循环时，更大的联接缓冲区可能是有益的，直到第一个表中所有行的所有必需列都存储在联接缓冲区中。这取决于查询；最佳大小可以小于保持来自第一表的所有行。

使用批量密钥访问时，join_buffer_size的值定义了向存储引擎发出的每个请求中密钥的批量大小。缓冲区越大，对联接操作的右侧表的顺序访问就越多，这可以显著提高性能。

有关连接缓冲的更多信息，请参阅第8.2.1.6节“嵌套循环连接算法”。有关批量密钥访问的信息，请参阅第8.2.1.11节“块嵌套循环和批量密钥访问连接”。

## keep_files_on_create

> 保持文件处于创建状态

如果创建的MyISAM表没有DATA DIRECTORY选项，则。MYD文件是在数据库目录中创建的。默认情况下，如果MyISAM找到现有的。在这种情况下，它会覆盖MYD文件。这同样适用于。不使用INDEX DIRECTORY选项创建的表的MYI文件。要抑制此行为，请将keep_files_on_create变量设置为on（1），在这种情况下，MyISAM不会覆盖现有文件，而是返回一个错误。默认值为OFF（0）。

如果MyISAM表是使用DATA DIRECTORY或INDEX DIRECTORY选项和现有的创建的。MYD或。如果找到MYI文件，MyISAM总是返回一个错误。它不会覆盖指定目录中的文件。

## key_buffer_size

> 密钥缓冲区大小

MyISAM表的索引块是缓冲的，并由所有线程共享。key_buffer_size是用于索引块的缓冲区的大小。密钥缓冲区也称为密钥缓存。

允许的最小设置为0，但不能动态地将key_buffer_size设置为0。设置为0将删除密钥缓存，这在运行时是不允许的。只有在启动时才允许将key_buffer_size设置为0，在这种情况下，密钥缓存不会初始化。在运行时将key_buffer_size设置从值0更改为允许的非零值将初始化密钥缓存。

key_buffer_size只能以4096字节的增量或倍数增加或减少。通过不合格值增加或减少设置会产生警告，并将设置截断为合格值。

在32位平台上，key_buffer_size的最大允许设置为4GB−1。64位平台允许使用更大的值。有效的最大大小可能会更小，这取决于您的可用物理RAM和操作系统或硬件平台对每个进程的RAM限制。此变量的值表示请求的内存量。在内部，服务器会分配尽可能多的内存，但实际分配的内存可能会更少。

您可以增加该值以更好地处理所有读取和多次写入的索引；在一个主要功能是使用MyISAM存储引擎运行MySQL的系统上，该变量可以接受机器总内存的25%。但是，您应该注意，如果您使该值过大（例如，超过机器总内存的50%），系统可能会开始分页并变得非常缓慢。这是因为MySQL依赖于操作系统来执行数据读取的文件系统缓存，所以必须为文件系统缓存留出一些空间。除了MyISAM之外，您还应该考虑可能使用的任何其他存储引擎的内存需求。

为了在同时写入多行时获得更高的速度，请使用LOCK TABLES。请参阅第8.2.4.1节“优化INSERT语句”。

您可以通过发出SHOW STATUS语句并检查key_read_requests、key_reads、key_write_requests和key_writes状态变量来检查密钥缓冲区的性能。（参见第13.7.5节“SHOW语句”。）Key_reads/Key_read_requests之比通常应小于0.01。如果您主要使用更新和删除，Key_write_requests的比率通常接近1，但如果您倾向于同时进行影响多行的更新，或者如果您使用DELAY_Key_write表选项，则比率可能会小得多。

可以使用key_buffer_size结合key_block_unused状态变量和缓冲块大小来确定所使用的密钥缓冲区的分数，该缓冲块大小可从key_cache_block_size系统变量获得：

```sql
1 - ((Key_blocks_unused * key_cache_block_size) / key_buffer_size)
```

这个值是近似值，因为密钥缓冲区中的一些空间是在内部分配给管理结构的。影响这些结构的开销量的因素包括块大小和指针大小。随着块大小的增加，由于开销而丢失的密钥缓冲区的百分比往往会降低。较大的块会导致较少的读取操作次数（因为每次读取会获得更多的密钥），但相反，会增加未检查的密钥的读取次数（如果不是块中的所有密钥都与查询相关）。

可以创建多个MyISAM密钥缓存。4GB的大小限制单独应用于每个缓存，而不是作为一个组。请参阅第8.10.2节“MyISAM密钥缓存”。

## key_cache_age_threshold

> 密钥缓存使用期限阈值

此值控制缓冲区从密钥缓存的热子列表降级到热子列表。值越低，降级发生得越快。最小值为100。默认值为300。请参阅第8.10.2节“MyISAM密钥缓存”。

## key_cache_block_size

> 密钥缓存块大小

密钥缓存中块的大小（以字节为单位）。默认值为1024。请参阅第8.10.2节“MyISAM密钥缓存”。

## key_cache_division_limit

> 密钥缓存划分限制

密钥缓存缓冲区列表的热子列表和热子列表之间的分界点。该值是用于暖子列表的缓冲区列表的百分比。允许值的范围从1到100。默认值为100。请参阅第8.10.2节“MyISAM密钥缓存”。

## keyring_operations

> 钥匙圈操作

此参数设置是否允许对innodb表空间加密所用的秘钥进行迁移等操作。

## large_files_support

> 大文件支持

是否使用支持大文件的选项编译了mysqld。

## large_pages

> 大页面

是否启用大页面支持（通过--large pages选项）。请参阅第8.12.4.3节“启用大页面支持”。

## large_page_size

> 大页面大小

如果启用了大页面支持，则显示内存页面的大小。只有Linux才支持大内存页；在其他平台上，此变量的值始终为0。请参阅第8.12.4.3节“启用大页面支持”。

## last_insert_id

> 上次插入id

从LAST_INSERT_ID（）返回的值。当您在更新表的语句中使用LAST_INSERT_ID（）时，它会存储在二进制日志中。设置此变量不会更新mysql_insert_id（）C API函数返回的值。

## lc_messages

> lc消息

用于错误消息的区域设置。默认值为en_US。服务器将参数转换为语言名称，并将其与lc_messages_dir的值组合，以生成错误消息文件的位置。请参阅第10.12节“设置错误消息语言”。

## lc_messages_dir

> lc消息目录

错误消息所在的目录。服务器将该值与lc_messages的值一起用于生成错误消息文件的位置。请参阅第10.12节“设置错误消息语言”。

## lc_time_names

> lc时间名称

此变量指定区域设置，该区域设置控制用于显示日期和月份名称及缩写的语言。此变量影响DATE_FORMAT（）、DAYNAME（）和MONTHNAME（）函数的输出。区域设置名称是POSIX样式的值，如“ja_JP”或“pt_BR”。无论系统的区域设置如何，默认值都是“en_US”。有关更多信息，请参阅第10.16节“MySQL Server区域设置支持”。

## license

> 许可证

服务器拥有的许可证类型。

## local_infile

> 局部内野

此变量控制LOAD DATA语句的服务器端LOCAL功能。根据local_infile设置，服务器拒绝或允许在客户端启用了local的客户端加载本地数据。

要明确地导致服务器拒绝或允许LOAD DATA LOCAL语句（无论在构建时或运行时如何配置客户端程序和库），请分别在禁用或启用LOCAL_infile的情况下启动mysqld。local_infile也可以在运行时设置。有关更多信息，请参阅第6.1.6节“本地加载数据的安全注意事项”。

## lock_wait_timeout

> 锁定等待超时

此变量指定尝试获取元数据锁的超时时间（以秒为单位）。允许值的范围从1到31536000（1年）。默认值为31536000。

- 此超时适用于所有使用元数据锁的语句。其中包括对表、视图、存储过程和存储函数的DML和DDL操作，以及LOCK tables、FLUSH tables WITH READ LOCK和HANDLER语句。

- 此超时不适用于对mysql数据库中系统表的隐式访问，例如由grant或REVOKE语句或表日志记录语句修改的grant表。超时确实适用于直接访问的系统表，例如使用SELECT或UPDATE。

超时值分别应用于每次元数据锁定尝试。给定的语句可能需要多个锁，因此在报告超时错误之前，该语句可能会阻塞超过lock_wait_timeout值的时间。锁定超时时，报告ER_lock_WAIT_timeout。

lockwait_timeout不适用于延迟插入，延迟插入总是在超时1年的情况下执行。这样做是为了避免不必要的超时，因为发出延迟插入的会话不会收到延迟插入超时的通知。

## log_bin

<https://dev.mysql.com/doc/refman/5.7/en/replication-options-binary-log.html>

## log_error

> 日志错误

错误日志输出目标。如果目标是控制台，则值为stderr。否则，目标是一个文件，log_error值是文件名。参见第5.4.2节“错误日志”。

## log_error_verbosity

> 日志错误详细程度

服务器在向错误日志中写入错误、警告和注释消息时的详细程度。下表显示了允许的值。默认值为3。

log_error_verbosity值 |Permitted Messages允许的消息
--|--
1

> Error messages 错误消息
2 |Error and warning messages 错误和警告消息
3 |Error, warning, and information messages 错误、警告和信息消息

在MySQL 5.7.2中添加了log_error_verbosity。它比旧的log_warnings系统变量更可取，并且应该使用它来代替旧的log_warnings系统。有关该变量如何与log_error_verbosity相关的信息，请参阅log_warnings的描述。特别是，为log_warnings分配值会为log_error_verbosity分配值，反之亦然。

## log_output

> 日志输出

常规查询日志和慢速查询日志输出的一个或多个目标。该值是从TABLE、FILE和NONE中选择的一个或多个逗号分隔单词的列表。TABLE选择对mysql系统数据库中的general_log和slow_log表进行日志记录。FILE选择记录以记录文件。NONE禁用日志记录。如果值中存在NONE，则它优先于存在的任何其他单词。TABLE和FILE都可以用于选择两个日志输出目的地。

此变量选择日志输出目标，但不启用日志输出。为此，请启用general_log和slow_query_log系统变量。对于FILE日志记录，general_log_FILE和slow_query_log_FILE系统变量确定日志文件的位置。有关更多信息，请参阅第5.4.1节“选择常规查询日志和慢速查询日志输出目的地”。

## log_queries_not_using_indexes

> 不使用索引的日志查询

如果在启用慢速查询日志的情况下启用此变量，则会记录预期检索所有行的查询。请参阅第5.4.5节“慢速查询日志”。此选项并不一定意味着不使用索引。例如，使用完整索引扫描的查询使用索引，但会被记录，因为索引不会限制行数。

## log_slave_updates

> 日志从属更新

## log_slow_admin_statements

> 记录慢速管理语句

在写入慢速查询日志的语句中包括慢速管理语句。管理语句包括ALTER TABLE、ANALYZE TABLE、CHECK TABLE、CREATE INDEX、DROP INDEX、OPTIMIZE TABLE和REPAIR TABLE。

## log_slow_slave_statements

> 记录慢速从属语句

## log_statements_unsafe_for_binlog

> 日志语句对binlog不安全

## log_syslog

> 日志系统日志

是否将错误日志输出写入系统日志。这是Windows上的事件日志，Unix和类Unix系统上的系统日志。默认值是特定于平台的：

- 在Windows上，默认情况下会启用事件日志输出。
- 在Unix和类Unix系统上，系统日志输出默认为禁用状态。

不管默认情况如何，log_syslog都可以显式设置为控制任何支持平台上的输出。

系统日志输出控制不同于将错误输出发送到文件或控制台。根据需要，除了系统日志之外，还可以将错误输出定向到文件或控制台，或者不定向到系统日志。参见第5.4.2节“错误日志”。

## log_syslog_facilitylog

将错误日志输出写入系统日志的功能（发送消息的程序类型）。除非启用了log_syslog系统变量，否则此变量无效。参见第5.4.2.3节“系统日志的错误记录”。

允许的值可能因操作系统而异；请参阅系统syslog文档。

此变量在Windows上不存在。

## log_syslog_include_pid

是否在写入syslog的错误日志输出的每一行中包括服务器进程ID。除非启用了log_syslog系统变量，否则此变量无效。参见第5.4.2.3节“系统日志的错误记录”。

此变量在Windows上不存在。

## log_syslog_tag

> log syslog标记

要添加到写入syslog的错误日志输出中的服务器标识符的标记。除非启用了log_syslog系统变量，否则此变量无效。参见第5.4.2.3节“系统日志的错误记录”。

默认情况下，服务器标识符是不带标记的mysqld。如果指定了tag的标记值，则会使用前导连字符将其附加到服务器标识符，从而生成mysqld标记的标识符。

在Windows上，要使用不存在的标记，必须从具有管理员权限的帐户运行服务器，才能为标记创建注册表项。如果标记已经存在，则不需要提升权限。

## log_throttle_queries_not_using_indexes

> 不使用索引的日志限制查询

如果启用了log_queries_not_using_indexes，则log_throtte_queries_not_using_inindexes变量会限制每分钟可写入慢速查询日志的此类查询的数量。值0（默认值）表示“无限制”。有关更多信息，请参阅第5.4.5节“慢速查询日志”。

## log_timestamps

> 日志时间戳

此变量控制写入错误日志的消息中的时间戳的时区，以及通常写入文件的查询日志和慢速查询日志消息中的时区。它不影响写入表（mysql.general_log，mysql.slow_log）的常规查询日志和慢速查询日志消息的时区。从这些表中检索的行可以通过CONVERT_TZ（）或设置会话time_zone系统变量从本地系统时区转换为任何所需时区。

允许的log_timestamp值为UTC（默认值）和SYSTEM（本地系统时区）。

时间戳使用ISO 8601/RFC 3339格式编写：YYYY MM DDThh:MM:ss.uuuuuu加上表示祖鲁时间（UTC）或±hh:MM（与UTC的偏移量）的Z尾值。

## log_warnings

> 日志警告

是否向错误日志生成其他警告消息。从MySQL 5.7.2开始，以前由log_warnings管理的信息项由log_error_verbosity管理，它优先于旧的log_warning系统变量，并且应该使用它来代替旧的log_warnings系统变量。（不赞成使用log_warnings系统变量和--log warnings命令行选项；希望在MySQL的未来版本中删除它们。）

log_warnings默认启用（MySQL 5.7.2之前默认为1，自5.7.2起为2）。要禁用它，请将其设置为0。如果该值大于0，则服务器会记录有关语句的消息，这些语句对于基于语句的日志记录是不安全的。如果该值大于1，则服务器会记录新连接尝试的中止连接和拒绝访问错误。请参阅第B.3.2.9节“通信错误和中止的连接”。

如果使用复制，建议通过将该变量设置为大于0来启用该变量，以获取有关正在发生的情况的更多信息，例如有关网络故障和重新连接的消息。

如果复制副本服务器是在启用log_warnings的情况下启动的，则复制副本会将消息打印到错误日志中，以提供有关其状态的信息，例如二进制日志和中继日志坐标，它启动作业的位置、切换到另一个中继日志的时间、断开连接后重新连接的时间等等。

为log_warnings赋值会为log_error_verbosity赋值，反之亦然。这些变量的关系如下：

- 在log_warnings=0时实现的所有log_warning项的抑制，在log_error_verbosity=1时实现（仅限错误）。

- 为log_warnings=1或更高级别打印的项目将被视为警告，为log_error_verbosity=2或更高版本打印的项目。
- 为log_warnings=2打印的项目算作注释，为log_error_verbosity=3打印的项目。

从MySQL 5.7.2开始，默认日志级别由log_error_verbosity控制，默认值为3。此外，log_warnings的默认值从1更改为2，对应于log_error_verbosity=3。要实现与以前默认值类似的日志记录级别，请将log_error_verbosity=2设置为。

在MySQL 5.7.2及更高版本中，仍然允许使用log_warnings，但映射到log_error_verbosity的使用，如下所示：

- 设置log_warnings=0相当于log_error_verbosity=1（仅限错误）。
- 设置log_warnings=1相当于log_error_verbosity=2（错误、警告）。
- 设置log_warnings=2（或更高）相当于log_error_verbosity=3（错误、警告、注释），如果指定了更大的值，则服务器会将log_warning设置为2。
  
## long_query_time

> 查询时间长

如果查询花费的时间超过此秒数，则服务器会递增Slow_queries状态变量。如果启用了慢速查询日志，则会将查询记录到慢速查询日志文件中。该值是实时测量的，而不是CPU时间，因此在轻负载系统上低于阈值的查询可能在重负载系统上高于阈值。long_query_time的最小值和默认值分别为0和10。最大值为31536000，即365天（秒）。该值可以指定为微秒的分辨率。请参阅第5.4.5节“慢速查询日志”。

此变量的值越小，则会有更多的语句被认为是长时间运行的，因此慢速查询日志需要更多的空间。对于非常小的值（小于1秒），日志可能会在很短的时间内增长得很大。增加被视为长时间运行的语句数量也可能导致MySQL Enterprise Monitor中“长时间运行进程数量过多”警报的误报，尤其是在启用了组复制的情况下。由于这些原因，非常小的值应该仅在测试环境中使用，或者在生产环境中仅在短时间内使用。

## low_priority_updates

> 低优先级更新

如果设置为1，则所有INSERT、UPDATE、DELETE和LOCK TABLE WRITE语句都会等待，直到受影响的表上没有挂起的SELECT或LOCK TABLE READ。使用`｛INSERT |REPLACE| DELETE| UPDATE｝LOW_PRIORITY...`也可以获得相同的效果。 以降低仅一个查询的优先级。此变量仅影响仅使用表级锁定的存储引擎（如MyISAM、MEMORY和MERGE）。参见第8.11.2节“表格锁定问题”。

## lower_case_file_system

> 大小写文件系统

此变量描述数据目录所在的文件系统上文件名的大小写敏感性。OFF表示文件名区分大小写，ON表示不区分大小写。此变量是只读的，因为它反映了文件系统属性，并且设置它对文件系统没有影响。

## lower_case_table_names

> 大小写是否敏感

如果设置为0，则表名将按指定存储，并且比较区分大小写。如果设置为1，则表名以小写形式存储在磁盘上，并且比较不区分大小写。如果设置为2，则表名按给定值存储，但比较时使用小写字母。此选项也适用于数据库名称和表别名。有关更多详细信息，请参阅第9.2.3节“标识符大小写敏感性”。

此变量的默认值取决于平台（请参阅lower_case_file_system）。在Linux和其他类似Unix的系统上，默认值为0。在Windows上，默认值为1。在macOS上，默认值为2。在Linux（和其他类似Unix的系统）上，不支持将值设置为2；服务器将强制该值为0。

如果在数据目录位于不区分大小写的文件系统（如Windows或macOS）上的系统上运行MySQL，则不应将lower_case_table_names设置为0。这是一个不受支持的组合，在运行INSERT INTO时可能会导致挂起条件。。。选择。。。使用错误的tbl_name字母大小写进行FROM tbl_name操作。使用MyISAM，使用不同的字母大小写访问表名可能会导致索引损坏。

如果您试图在不区分大小写的文件系统上以--lower_case_table_names=0启动服务器，则会打印一条错误消息，并退出服务器。

此变量的设置会影响复制筛选选项在区分大小写方面的行为。有关更多信息，请参阅第16.2.5节“服务器如何评估复制筛选规则”。

## master_info_repository

> 主信息存储库

## master_verify_checksum

> 主校验和

## max_allowed_packet

> 最大允许数据包

一个数据包或任何生成/中间字符串的最大大小，或`mysql_stmt_send_long_data()` C API函数发送的任何参数。默认值为4MB。

数据包消息缓冲区初始化为net_buffer_length字节，但在需要时可以增加到max_allowed_packet字节。默认情况下，此值较小，用于捕获较大（可能不正确）的数据包。

如果使用大型BLOB列或长字符串，则必须增加此值。它应该和您想要使用的最大BLOB一样大。最大允许数据包的协议限制为1GB。该值应该是1024的倍数；非倍数被四舍五入到最接近的倍数。

通过更改max_allowed_packet变量的值来更改消息缓冲区大小时，如果客户端程序允许，还应更改客户端的缓冲区大小。客户端库中内置的默认max_allowed_packet值为1GB，但个别客户端程序可能会覆盖此值。例如，mysql和mysqldump的默认值分别为16MB和24MB。它们还允许您通过在命令行或选项文件中设置max_allowed_packet来更改客户端值。

此变量的会话值是只读的。客户端最多可以接收与会话值一样多的字节。但是，服务器向客户端发送的字节数不能超过当前全局max_allowed_packet值。（如果在客户端连接后更改了全局值，则全局值可能小于会话值。）

## max_binlog_cache_size

> binlog缓存的最大大小
>
## max_binlog_size

> 最大binlog大小
>
## max_binlog_stmt_cache_size

> 最大binlog stmt缓存大小
>
## max_connect_errors

> 最大连接错误

在max_connect_errors之后，来自主机的连续连接请求在没有成功连接的情况下被中断，服务器会阻止该主机进行进一步的连接。如果在前一个连接中断后，在少于max_connect_errors尝试的时间内成功建立了与主机的连接，则主机的错误计数将清除为零。要解除阻止被阻止的主机，请刷新主机缓存；请参阅[刷新主机缓存](https://dev.mysql.com/doc/refman/5.7/en/host-cache.html#host-cache-flushing)。

## max_connections

> 最大连接数

同时允许的最大客户端连接数。最大有效值是open_files_limit-810的有效值和实际为max_connections设置的值中的较小值。

有关更多信息，请参阅[第5.1.1.1节“连接接口”](https://dev.mysql.com/doc/refman/5.7/en/connection-interfaces.html)。

## max_delayed_threads

> 最大延迟线程数

不赞成使用此系统变量（因为不支持DELAYED插入）；预计它将在未来的版本中删除。

## max_digest_length

> 最大摘要长度

每个会话为计算规范化语句摘要而保留的最大内存字节数。一旦在摘要计算过程中使用了该空间量，就会发生截断：解析语句中没有进一步的令牌被收集或计入其摘要值。只有在许多字节的解析令牌之后才不同的语句才会产生相同的规范化语句摘要，并且如果进行比较或聚合以获得摘要统计信息，则这些语句被认为是相同的。

**将max_dgest_length设置为零将禁用摘要生产，这也将禁用需要摘要的服务器功能，如MySQL企业防火墙。**

减小max_digist_length值可以减少内存使用，但如果更多语句的摘要值仅在末尾不同，则会导致它们变得不可区分。增加该值可以区分较长的语句，但会增加内存使用量，尤其是对于涉及大量同时会话的工作负载（服务器为每个会话分配max_digest_length字节）。

解析器使用这个系统变量来限制它计算的规范化语句摘要的最大长度。如果性能模式跟踪语句摘要，则会使用Performance_Schema_max_digest_length复制摘要值。系统变量，作为对其存储的摘要的最大长度的限制。因此，如果performance_schema_max_dgest_length小于max_dgesT_length，则存储在性能模式中的摘要值相对于原始摘要值被截断。

有关语句消化的更多信息，请参阅[第25.10节“性能模式语句消化”](https://dev.mysql.com/doc/refman/5.7/en/performance-schema-statement-digests.html)。

## max_error_count

> 最大错误计数

SHOW ERRORS和SHOW WARNINGS语句要存储以供显示的错误、警告和信息消息的最大数量。这与诊断区域中的状况区域数量相同，因此也与GET diagnostics可以检查的状况数量相同。

## max_execution_time

> 最大执行时间  0~ 4294967295毫秒  大概5天不到

SELECT语句的执行超时，以毫秒为单位。如果该值为0，则不会启用超时。

max_execution_time应用如下：

- 全局max_execution_time值为新连接的会话值提供默认值。会话值适用于在不包含MAX_EXECUTION_TIME（N）优化器提示或N为0的会话中执行的SELECT执行。
- max_execution_time应用于只读SELECT语句。非只读语句是指那些调用存储函数的语句，该函数将修改数据作为副作用。
- 对于存储程序中的SELECT语句，将忽略max_execution_time。

## max_heap_table_size

> 最大堆表大小

此变量设置允许用户创建的MEMORY表增长的最大大小。变量的值用于计算MEMORY表MAX_ROWS值。

设置此变量对任何现有MEMORY表都没有影响，除非使用CREATE table等语句重新创建该表，或者使用ALTER table或TRUNCATE table更改该表。服务器重新启动还会将现有MEMORY表的最大大小设置为全局max_heap_table_size值。

此变量还与tmp_table_size一起使用，以限制内存中内部表的大小。请参阅第8.4.4节“MySQL中的内部临时表使用”。

未复制max_heap_table_size。有关更多信息，请参阅第16.4.1.20节“复制和MEMORY表”和第16.4.1.37节“复制与变量”。

## max_insert_delayed_threads

> 最大插入延迟线程数

此变量是max_delayerd_threads的同义词。

不赞成使用此系统变量（因为不支持DELAYED插入）；预计它将在未来的版本中删除。

## max_join_size

> 最大联接大小

不允许可能需要检查超过max_join_size行（对于单表语句）或行组合（对于多表语句）的语句，或者可能执行超过max_join_size磁盘查找的语句。通过设置此值，您可以捕获键使用不正确的语句，这可能需要很长时间。如果用户倾向于执行缺少WHERE子句、耗时较长或返回数百万行的联接，请设置它。有关详细信息，请参阅使用安全更新模式（--Safe Updates）。

将此变量设置为DEFAULT以外的值会将sql_big_selects的值重置为0。如果再次设置sql_big_selects值，则会忽略max_join_size变量。

如果查询结果在查询缓存中，则不执行结果大小检查，因为该结果之前已经计算过，并且不会给服务器带来将其发送到客户端的负担。

## max_length_for_sort_data

> 排序数据的最大长度

索引值大小的截止值，用于确定要使用的文件排序算法。参见第8.2.1.14节“按优化排序”。

## max_points_in_geometry

> 几何图形中的最大点

ST_Buffer_Strategy（）函数的points_per_circle参数的最大值。

## max_prepared_stmt_count

> 最大准备stmt计数

此变量限制服务器中准备语句的总数。它可以用于有可能因准备大量语句导致服务器内存不足而遭到拒绝服务攻击的环境。如果该值设置为低于当前已准备语句的数量，则现有语句不受影响，可以使用，但在当前数量降至限制以下之前，不能准备新语句。将该值设置为0将禁用准备好的语句。

## max_relay_log_size

> 最大中继日志大小

## max_seeks_for_key

> max寻找密钥

根据关键字查找行时，限制假定的最大寻道次数。MySQL优化器假设，无论索引的实际基数如何，当通过扫描索引来搜索表中的匹配行时，所需的关键字搜索次数不超过此数量（请参阅第13.7.5.22节“SHOW index语句”）。通过将其设置为较低的值（例如100），可以强制MySQL更喜欢索引而不是表扫描。

## max_sort_length

> 最大排序长度

对数据值进行排序时要使用的字节数。服务器只使用每个值的第一个max_sort_length字节，而忽略其余字节。因此，对于GROUP BY、ORDER BY和DISTINCT操作，只有在第一个max_sort_lengh字节之后才不同的值比较为相等。

增加max_sort_length的值可能也需要增加sort_buffer_size的值。有关详细信息，请参阅第8.2.1.14节“按优化排序”

## max_sp_recursion_depth

> 最大sp递归深度

可以递归调用任何给定存储过程的次数。此选项的默认值为0，这将完全禁用存储过程中的递归。最大值为255。

存储过程递归增加了对线程堆栈空间的需求。如果增加max_sp_recursion_depth的值，则可能需要在服务器启动时通过增加thread_stack的值来增加线程堆栈大小。

## max_tmp_tables

> 最大tmp表

此变量未使用。它已被弃用，并在MySQL 8.0中被删除。

## max_user_connections

> 最大用户连接数

任何给定MySQL用户帐户允许的最大同时连接数。值0（默认值）表示“无限制”

此变量具有全局值，该值可以在服务器启动或运行时设置。它还有一个只读会话值，指示适用于与当前会话关联的帐户的有效同时连接限制。会话值初始化如下：

- 如果用户帐户的MAX_user_CONNECTIONS资源限制为非零，则会话MAX_user_CONNECTIONS值将设置为该限制。
- 否则，会话max_user_connections值将设置为全局值。

帐户资源限制是使用CREATE USER或ALTER USER语句指定的。参见第6.2.16节“设置帐户资源限制”。

## max_write_lock_count

> 最大写入锁定计数

在这么多写锁之后，允许在其间处理一些挂起的读锁请求。写入锁定请求的优先级高于读取锁定请求。然而，如果max_write_lock_count被设置为某个低值（例如，10），则如果读取锁定请求已经被传递以支持10个写入锁定请求，则读取锁定请求可能比挂起的写入锁定请求更可取。通常不会发生这种行为，因为默认情况下max_write_lock_count的值非常大。

## mecab_rc_file

> mecab rc文件

mecab_rc_file选项用于设置mecab全文分析器。

mecab_rc_file选项定义mecabrc配置文件的路径，该文件是mecab的配置文件。该选项是只读的，只能在启动时设置。初始化MeCab需要mecabrc配置文件。

有关MeCab全文分析器的信息，请参阅第12.9.9节“MeCab完整文本分析器插件”。

## metadata_locks_cache_size

> 元数据锁定缓存大小

元数据锁定缓存的大小。服务器使用此缓存来避免创建和销毁同步对象。这在诸如Windows XP之类的操作成本高昂的系统上尤其有用。

在MySQL 5.7.4中，元数据锁定实现的更改使该变量变得不必要，因此不推荐使用；期望它在MySQL的未来版本中被删除。

## metadata_locks_hash_instances

> 元数据锁定哈希实例

元数据锁集可以划分为单独的散列，以允许访问不同对象的连接使用不同的锁定散列并减少争用。metadata_locks_hash_instances系统变量指定哈希数（默认为8）。

在MySQL 5.7.4中，元数据锁定实现的更改使该变量变得不必要，因此不推荐使用；期望它在MySQL的未来版本中被删除。

## min_examined_row_limit

> 最小检查行限制

检查少于此行数的查询不会记录到慢速查询日志中。

## multi_range_count

> 多量程计数

此变量没有影响。它已被弃用，并在MySQL 8.0中被删除。

## myisam_data_pointer_size

> myisam数据指针大小

以字节为单位的默认指针大小，当未指定MAX_ROWS选项时，CREATE TABLE将用于MyISAM表。此变量不能小于2或大于7。默认值为6。请参阅B.3.2.10节，“表格已满”。

## myisam_max_sort_file_size

> myisam最大排序文件大小

MySQL在重新创建MyISAM索引时（在REPAIR TABLE、ALTER TABLE或LOAD DATA期间）允许使用的临时文件的最大大小。如果文件大小大于此值，则使用键缓存创建索引，这会更慢。该值以字节为单位。

如果MyISAM索引文件超过此大小并且磁盘空间可用，则增加该值可能有助于提高性能。该空间必须在包含原始索引文件所在目录的文件系统中可用。

## myisam_mmap_size

> myisam mmap大小

用于内存映射压缩的MyISAM文件的最大内存量。如果使用许多压缩的MyISAM表，则可以减小该值以降低内存交换问题的可能性。

## myisam_recover_options

> myisam恢复选项

设置MyISAM存储引擎恢复模式。变量值是OFF、DEFAULT、BACKUP、FORCE或QUICK值的任意组合。如果指定了多个值，请用逗号分隔。在服务器启动时指定没有值的变量与指定DEFAULT相同，使用显式值“”指定会禁用恢复（与值OFF相同）。如果启用了恢复，则每次mysqld打开MyISAM表时，都会检查该表是否标记为已崩溃或未正确关闭。（最后一个选项仅在禁用外部锁定的情况下运行时有效。）如果是这种情况，mysqld会对表进行检查。如果表已损坏，mysqld会尝试修复它。

以下选项会影响修复的工作方式。

Option 选项|Description 描述
--|--
OFF 关闭| No recovery. 没有恢复。
DEFAULT 违约 |Recovery without backup, forcing, or quick checking. 无需备份、强制或快速检查即可恢复。
BACKUP 备份|If the data file was changed during recovery, save a backup of the ***tbl_name***.MYD file as ***tbl_name-datetime***.BAK. 如果数据文件在恢复过程中发生了更改，请保存tbl_name的备份。MYD文件为tbl_name-datetime。BAK。
FORCE 力|Run recovery even if we would lose more than one row from the .MYD file. 即使我们会从中丢失多行，也要运行恢复。MYD文件。
QUICK 快速的

> Do not check the rows in the table if there are not any delete blocks. 如果没有任何删除块，请不要检查表中的行。

在服务器自动修复表之前，它会在错误日志中写入有关修复的说明。如果希望能够在无需用户干预的情况下从大多数问题中恢复，则应使用选项BACKUP、FORCE。这会强制修复表，即使某些行会被删除，但它会将旧的数据文件作为备份，以便您以后可以检查发生了什么。

请参阅第15.2.1节“MyISAM启动选项”。

## myisam_sort_buffer_size

> myisam排序缓冲区大小

在REPAIR TABLE期间对MyISAM索引进行排序或使用CREATE INDEX或ALTER TABLE创建索引时分配的缓冲区大小。

## myisam_stats_method

> myisam统计方法

在收集有关MyISAM表的索引值分布的统计信息时，服务器如何处理NULL值。此变量有三个可能的值，nulls_equal、nulls_invariable和nulls_ignored。对于nulls_equal，所有NULL索引值都被视为相等，并形成一个大小等于NULL值数量的单个值组。对于nulls_equival，NULL值被认为是不相等的，并且每个NULL形成大小为1的不同值组。对于nulls_igned，将忽略NULL值。

用于生成表统计信息的方法会影响优化器为查询执行选择索引的方式，如第8.3.7节“InnoDB和MyISAM索引统计信息集合”所述。

## myisam_use_mmap

> myisam使用mmap

使用内存映射读取和写入MyISAM表。

## mysql_native_password_proxy_users

> mysql本机密码代理用户

此变量控制mysql_native_password内置身份验证插件是否支持代理用户。除非启用了check_proxy_users系统变量，否则它将无效。有关用户代理的信息，请参阅第6.2.14节“代理用户”。

## named_pipe

> 命名管道

（仅限Windows。）指示服务器是否支持通过命名管道进行连接。

## named_pipe_full_access_group

> 命名管道完全访问组

（仅限Windows。）当named_pipe系统变量被启用以支持命名管道连接时，在MySQL服务器创建的命名管道上授予客户端的访问控制被设置为成功通信所需的最小值。一些MySQL客户端软件可以在没有任何额外配置的情况下打开命名管道连接；然而，其他客户端软件可能仍然需要完全访问才能打开命名管道连接。

此变量设置Windows本地组的名称，MySQL服务器授予其成员足够的访问权限以使用命名管道客户端。从MySQL 5.7.34开始，默认值设置为空字符串，这意味着没有Windows用户被授予对命名管道的完全访问权限。

可以在Windows中创建一个新的Windows本地组名称（例如，mysql_access_client_users），然后在绝对需要访问时用于替换默认值。在这种情况下，请将组的成员资格限制为尽可能少的用户，以便在升级用户的客户端软件时将其从组中删除。在Windows管理员将用户添加到组之前，尝试使用受影响的命名管道客户端打开MySQL连接的非组成员将被拒绝访问。新添加的用户必须注销并重新登录才能加入组（Windows要求）。

将值设置为“*everyone*”提供了一种独立于语言的方式来引用Windows上的everyone组。默认情况下，Everyone组不安全。

## net_buffer_length

> 净缓冲区长度

每个客户端线程都与一个连接缓冲区和结果缓冲区相关联。两者都以net_buffer_length给定的大小开始，但根据需要动态放大到max_allowed_packet字节。在每条SQL语句之后，结果缓冲区收缩为net_buffer_length。

该变量通常不应更改，但如果内存非常少，则可以将其设置为客户端发送的语句的预期长度。如果语句超过此长度，连接缓冲区将自动扩大。可以设置net_buffer_length的最大值为1MB。

此变量的会话值是只读的。

## net_read_timeout

> 网络读取超时

在中止读取之前等待来自连接的更多数据的秒数。当服务器从客户端读取时，net_read_timeout是控制何时中止的超时值。当服务器向客户端写入时，net_write_timeout是控制何时中止的超时值。另请参见slave_net_timeout。

## net_retry_count

> 净重试计数

如果通信端口上的读取或写入被中断，请在放弃之前重试多次。这个值应该在FreeBSD上设置得很高，因为内部中断被发送到所有线程。

## net_write_timeout

> 网络写入超时

在中止写入之前等待将块写入连接的秒数。另请参阅net_read_timeout。

## new

> 新

此变量在MySQL 4.0中用于启用某些4.1行为，并保留用于向后兼容性。其值始终为OFF。

在NDB Cluster中，将此变量设置为ON可以将KEY或LINERAL KEY以外的分区类型用于NDB表。此实验性功能在生产中不受支持，现在已被弃用，因此可能会在未来的版本中删除。有关其他信息，请参阅用户定义的分区和NDB存储引擎（NDB集群）。

## ngram_token_size

> ngram令牌大小

定义n-gram全文分析器的n-gram标记大小。ngram_token_size选项是只读的，只能在启动时修改。默认值为2（bigram）。最大值为10。

## offline_mode

> 脱机模式

服务器是否处于“脱机模式”，具有以下特征：

- 没有SUPER权限的已连接客户端用户在下一次请求时会断开连接，并出现相应的错误。断开连接包括终止正在运行的语句和释放锁。这样的客户端也不能发起新的连接，并且不能接收适当的错误。
- 具有SUPER权限的已连接客户端用户不会断开连接，并且可以启动新的连接来管理服务器。
- 只有具有SUPER权限的用户才能控制脱机模式。若要将服务器置于脱机模式，请将offline_mode系统变量的值从OFF更改为ON。若要恢复正常操作，请将offline_mode从ON更改为OFF。在脱机模式下，被拒绝访问的客户端会收到ER_server_offline_mode错误。

## old

> 老的

old是一个兼容性变量。它在默认情况下是禁用的，但可以在启动时启用，以将服务器恢复到旧版本中的行为。

当启用旧的时，它会将索引提示的默认范围更改为MySQL 5.1.17之前使用的范围。也就是说，不带FOR子句的索引提示仅适用于如何使用索引进行行检索，而不适用于ORDER BY或GROUP BY子句的解析。（请参阅第8.9.4节“索引提示”。）请注意在复制设置中启用此功能。对于基于语句的二进制日志记录，对源和副本使用不同的模式可能会导致复制错误。

## old_alter_table

> 旧的替换表

启用此变量时，服务器不使用优化的方法来处理ALTER TABLE操作。它恢复为使用临时表，复制数据，然后将临时表重命名为MySQL 5.0及更早版本使用的原始表。有关ALTER TABLE操作的更多信息，请参阅第13.1.8节“ALTER TABLE语句”。

## old_passwords

> 旧密码

MySQL 5.7中不赞成使用此系统变量；期望它在MySQL的未来版本中被删除。

此变量控制password（）函数使用的密码哈希方法。它还影响CREATE USER和GRANT语句执行的密码哈希，这些语句使用IDENTIFIED by子句指定密码。

下表显示了对于每个密码哈希方法，old_passwords的允许值以及哪些身份验证插件使用该哈希方法。

Password Hashing Method密码哈希方法 |old_passwords Valueold_passwords值 |Associated Authentication Plugin关联的身份验证插件
--|--|--
MySQL 4.1 native hashingMySQL 4.1本机哈希 |0 |mysql_native_passwordmysql_活动_密码
SHA-256 hashingSHA-256哈希 |2| sha256_passwordsha256_密码

如果将old_passwords设置为2，请按照第6.4.1.5节“SHA-256可插拔身份验证”中有关使用sha256_password插件的说明进行操作。

服务器在启动期间将全局old_passwords值设置为与default_authentication_plugin系统变量指示的身份验证插件所需的密码哈希方法一致。

当客户端成功连接到服务器时，服务器会为帐户身份验证方法适当地设置会话old_passwords值。例如，如果帐户使用sha256_password身份验证插件，则服务器会将old_passwords设置为2。

## open_files_limit

> 打开文件限制

操作系统中可用于mysqld的文件描述符数：

- 在启动时，mysqld使用setrlimit（）保留描述符，通过直接设置此变量或使用--open files limit选项将请求的值设置为mysqld_safe。如果mysqld产生错误“打开的文件太多”，请尝试增加open_files_limit值。在内部，此变量的最大值是最大无符号整数值，但实际最大值取决于平台。

- 在运行时，open_files_limit的值表示操作系统实际允许mysqld使用的文件描述符的数量，这可能与启动时请求的值不同。如果启动期间请求的文件描述符数量无法分配，mysqld会在错误日志中写入警告。

有效的open_files_limit值基于系统启动时指定的值（如果有）以及max_connections和table_open_cache的值，使用以下公式：

- 10+最大连接数+（table_open_cache*2）
- 最大连接数*5
- 操作系统限制，如果该限制为正，但不是无穷大。
- 如果操作系统限制为无穷大：如果在启动时指定了open_files_limit值，则为5000。

服务器尝试使用这些值的最大值来获取文件描述符的数量。如果不能获得那么多描述符，则服务器尝试获得系统允许的尽可能多的描述符。

在MySQL无法更改打开文件数的系统上，有效值为0。

在Unix上，该值不能设置为大于ulimit-n命令显示的值。在使用systemd的Linux系统上，该值不能设置为大于LimitNOFile（如果未设置LimitNOFile，则为DefaultLimitNOFILE）；否则，在Linux上，open_files_limit的值不能超过ulimit-n。

## optimizer_prune_level

> 优化器修剪级别

控制在查询优化期间应用的试探法，以从优化器搜索空间中删除不太有希望的部分计划。值为0将禁用启发式，以便优化器执行彻底搜索。值为1时，优化器会根据中间计划检索到的行数来修剪计划。

## optimizer_search_depth

> 优化器搜索深度

查询优化器执行的最大搜索深度。大于查询中关系数的值会产生更好的查询计划，但生成查询的执行计划需要更长的时间。小于查询中关系数的值可以更快地返回执行计划，但生成的计划可能远不是最佳的。如果设置为0，系统会自动选择一个合理的值。

## optimizer_switch

> 优化器开关

优化器开关系统变量可以控制优化器的行为。此变量的值是一组标志，每个标志的值为on或off，以指示相应的优化器行为是启用还是禁用。此变量具有全局值和会话值，可以在运行时更改。全局默认值可以在服务器启动时设置。

要查看当前的优化器标志集，请选择变量值：

```sql
mysql> SELECT @@optimizer_switch\G
*************************** 1. row ***************************
@@optimizer_switch: index_merge=on,index_merge_union=on,
                    index_merge_sort_union=on,
                    index_merge_intersection=on,
                    engine_condition_pushdown=on,
                    index_condition_pushdown=on,
                    mrr=on,mrr_cost_based=on,
                    block_nested_loop=on,batched_key_access=off,
                    materialization=on,semijoin=on,loosescan=on,
                    firstmatch=on,duplicateweedout=on,
                    subquery_materialization_cost_based=on,
                    use_index_extensions=on,
                    condition_fanout_filter=on,derived_merge=on,
                    prefer_ordering_index=on
```

有关此变量的语法及其控制的优化器行为的更多信息，请参阅[第8.9.2节“可切换优化”](https://dev.mysql.com/doc/refman/5.7/en/switchable-optimizations.html)。

## optimizer_trace

> 优化器跟踪

此变量控制优化器跟踪。有关详细信息，请参见MySQL内部：跟踪优化器。

## optimizer_trace_features

> 优化器跟踪功能

此变量启用或禁用选定的优化器跟踪功能。有关详细信息，请参见MySQL内部：跟踪优化器。

## optimizer_trace_limit

> 优化器跟踪限制

要显示的优化器跟踪的最大数目。有关详细信息，请参见MySQL内部：跟踪优化器。

## optimizer_trace_max_mem_size

> 优化器跟踪最大内存大小

存储的优化器跟踪的最大累积大小。有关详细信息，请参见MySQL内部：跟踪优化器。

## optimizer_trace_offset

> 优化器跟踪偏移

要显示的优化器跟踪的偏移量。有关详细信息，请参见MySQL内部：跟踪优化器。

## parser_max_mem_size

> 解析器最大内存大小

解析程序可用的最大内存量。默认值不限制可用内存。可以减少该值，以防止解析长或复杂的SQL语句时出现内存不足的情况。

## performance_schema

> 性能模式

[第25.15节“性能模式系统变量”](https://dev.mysql.com/doc/refman/5.7/en/performance-schema-system-variables.html)列出了性能模式的系统变量。这些变量可用于配置性能模式操作。

## performance_schema_accounts_size

> 性能架构帐户大小

## performance_schema_digests_size

> 性能模式摘要大小

## performance_schema_events_stages_history_long_size

> 性能模式事件阶段历史悠久

## performance_schema_events_stages_history_size

> 性能架构事件阶段历史记录大小

## performance_schema_events_statements_history_long_size

> 性能模式事件语句历史悠久

## performance_schema_events_statements_history_size

> 性能架构事件语句历史记录大小

## performance_schema_events_transactions_history_long_size

> 性能架构事件事务历史悠久

## performance_schema_events_transactions_history_size

> 性能架构事件事务历史记录大小

## performance_schema_events_waits_history_long_size

> 性能架构事件等待历史悠久

## performance_schema_events_waits_history_size

> 性能架构事件等待历史记录大小

## performance_schema_hosts_size

> 性能架构主机大小

## performance_schema_max_cond_classes

> 性能架构最大cond类

## performance_schema_max_cond_instances

> 性能架构最大秒实例

## performance_schema_max_digest_length

> 性能架构最大摘要长度

## performance_schema_max_file_classes

> 性能架构最大文件类

## performance_schema_max_file_handles

> 性能架构最大文件句柄

## performance_schema_max_file_instances

> 性能架构最大文件实例数

## performance_schema_max_index_stat

> 性能架构最大索引stat

## performance_schema_max_memory_classes

> 性能架构最大内存类

## performance_schema_max_metadata_locks

> 性能架构最大元数据锁

## performance_schema_max_mutex_classes

> 性能模式最大互斥类

## performance_schema_max_mutex_instances

> 性能模式最大互斥实例数

## performance_schema_max_prepared_statements_instances

> 性能架构最大准备语句实例

## performance_schema_max_program_instances

> 性能架构最大程序实例

## performance_schema_max_rwlock_classes

> 性能模式最大rwlock类

## performance_schema_max_rwlock_instances

> 性能架构最大rwlock实例

## performance_schema_max_socket_classes

> 性能架构最大套接字类

## performance_schema_max_socket_instances

> 性能架构最大套接字实例数

## performance_schema_max_sql_text_length

> 性能模式最大sql文本长度

## performance_schema_max_stage_classes

> 性能架构最大阶段类

## performance_schema_max_statement_classes

> 性能架构最大语句类

## performance_schema_max_statement_stack

> 性能模式最大语句堆栈

## performance_schema_max_table_handles

> 性能架构最大表句柄

## performance_schema_max_table_instances

> 性能架构最大表实例数

## performance_schema_max_table_lock_stat

> 性能架构最大表锁定stat

## performance_schema_max_thread_classes

> 性能架构最大线程类

## performance_schema_max_thread_instances

> 性能架构最大线程实例数

## performance_schema_session_connect_attrs_size

> 性能架构会话连接属性大小

## performance_schema_setup_actors_size

> 性能模式设置参与者大小

## performance_schema_setup_objects_size

> 性能架构设置对象大小

## performance_schema_show_processlist

> 性能模式显示进程列表

## performance_schema_users_size

> 性能架构用户大小

## pid_file

> pid文件

服务器写入进程ID的文件的路径名。除非指定了绝对路径名以指定其他目录，否则服务器会在数据目录中创建文件。如果指定此变量，则必须指定一个值。如果不指定此变量，MySQL将使用默认值host_name.pid，其中host_name是主机的名称。

进程ID文件由其他程序（如mysqld_safe）用于确定服务器的进程ID。在Windows上，此变量还会影响默认的错误日志文件名。参见第5.4.2节“错误日志”。

## plugin_dir

> 插件目录

插件目录的路径名。

如果插件目录可由服务器写入，则用户可以使用SELECT…将可执行代码写入目录中的文件。。。进入垃圾堆。这可以通过使plugin_dir对服务器只读或将secure_file_priv设置为可以安全进行SELECT写入的目录来防止。

## port

> 端口

服务器侦听TCP/IP连接的端口号。此变量可以使用--port选项进行设置。

## preload_buffer_size

> 预加载缓冲区大小

预加载索引时分配的缓冲区的大小。

## profiling

> 剖析

如果设置为0或OFF（默认值），则禁用语句分析。如果设置为1或ON，则启用语句评测，SHOW PROFILE和SHOW PROFILES语句提供对评测信息的访问。参见第13.7.5.31节“SHOW PROFILES声明”。

此变量已弃用；期望它在MySQL的未来版本中被删除。

## profiling_history_size

> 分析历史记录大小

如果启用了分析，则要维护其分析信息的语句数。默认值为15。最大值为100。将该值设置为0将有效地禁用分析。参见第13.7.5.31节“SHOW PROFILES声明”。

此变量已弃用；期望它在MySQL的未来版本中被删除。

## protocol_version

> 协议版本

MySQL服务器使用的客户端/服务器协议的版本。

## proxy_user

> 代理用户

如果当前客户端是另一个用户的代理，则此变量为代理用户帐户名。否则，此变量为NULL。参见第6.2.14节“代理用户”。

## pseudo_slave_mode

> 伪从属模式

此系统变量供内部服务器使用。pseudo_slave_mode有助于正确处理起源于比当前处理它们的服务器更旧或更新的服务器上的事务。mysqlbinlog在执行任何SQL语句之前将pseudo_slave_mode的值设置为true。

pseudo_slave_mode对已准备好的XA事务的处理有以下影响，这些事务可以附加到处理会话（默认情况下，发出XA START的会话）或从处理会话分离：

- 如果为true，并且处理会话已执行内部使用BINLOG语句，则事务的第一部分（直到XA PREPARE）一结束，XA事务就会自动从会话中分离，因此，具有XA_RECOVER_ADMIN权限的任何会话都可以提交或回滚XA事务。

- 如果为false，则只要处理会话处于活动状态，XA事务就会一直附加到该会话，在此期间，没有其他会话可以提交事务。只有在会话断开连接或服务器重新启动时，准备好的事务才会分离。

## pseudo_thread_id

> 伪线程id

此变量供内部服务器使用。

更改pseudo_thread_id系统变量的会话值会更改CONNECTION_id（）函数返回的值。

## query_alloc_block_size

> 查询分配块大小

为语句解析和执行期间创建的对象分配的内存块的分配大小（以字节为单位）。如果内存碎片有问题，增加此参数可能会有所帮助。

字节号的块大小为1024。在存储系统变量的值之前，MySQL Server会将不是块大小的精确倍数的值四舍五入到块大小的下一个较低倍数。解析器允许平台的最大无符号整数值（对于32位系统为4294967295或232−1，对于64位系统为18446744073709551615或264−1），但实际最大值要低一个块大小。

## query_cache_limit

> 查询缓存限制

不要缓存大于此字节数的结果。默认值为1MB。

从MySQL 5.7.20开始，查询缓存已被弃用，并在MySQL 8.0中被删除。弃用包括query_cache_limit。

## query_cache_min_res_unit

> 查询缓存最小res单位

查询缓存分配的块的最小大小（以字节为单位）。默认值为4096（4KB）。第8.10.3.3节“查询缓存配置”中给出了此变量的调整信息。

从MySQL 5.7.20开始，查询缓存已被弃用，并在MySQL 8.0中被删除。弃用包括query_cache_min_res_unit。

## query_cache_size

> 查询缓存大小

为缓存查询结果而分配的内存量。默认情况下，查询缓存处于禁用状态。这是使用默认值1M实现的，query_cache_type的默认值为0。（如果将大小设置为0，则要显著降低开销，还应在query_cache_type=0的情况下启动服务器。

允许值为1024的倍数；其他值则向下四舍五入到最接近的倍数。对于query_cache_size的非零值，即使query_cache_type=0，也会分配这么多字节的内存。有关更多信息，请参阅第8.10.3.3节“查询缓存配置”。

查询缓存至少需要大约40KB的大小来分配其结构。（具体大小取决于系统体系结构。）如果将query_cache_size的值设置得太小，则会出现警告，如第8.10.3.3节“查询缓存配置”所述。

从MySQL 5.7.20开始，查询缓存已被弃用，并在MySQL 8.0中被删除。弃用包括query_cache_size。

## query_cache_type

> 查询缓存类型

设置查询缓存类型。设置GLOBAL值将设置此后连接的所有客户端的类型。各个客户端可以设置SESSION值，以影响它们自己对查询缓存的使用。可能的值如下表所示。

Option选项| Description描述
--|--
0 or OFF  0或OFF |Do not cache results in or retrieve results from the query cache. Note that this does not deallocate the query cache buffer. To do that, you should set query_cache_size to 0.不要在查询缓存中缓存结果或从查询缓存中检索结果。请注意，这不会解除分配查询缓存缓冲区。为此，您应该将query_cache_size设置为0。
1 or ON  1或ON |Cache all cacheable query results except for those that begin with SELECT SQL_NO_CACHE.缓存除以SELECT SQL_NO_Cache开头的查询结果之外的所有可缓存查询结果。
2 or DEMAND  2或需求| Cache results only for cacheable queries that begin with SELECT SQL_CACHE.仅缓存以SELECT SQL_Cache开头的可缓存查询的结果。

此变量默认为OFF。

如果服务器在query_cache_type设置为0的情况下启动，则它根本不会获取查询缓存互斥，这意味着在运行时无法启用查询缓存，并且查询执行中的开销减少。

从MySQL 5.7.20开始，查询缓存已被弃用，并在MySQL 8.0中被删除。弃用包括query_cache_type。

## query_cache_wlock_invalidate

> 查询缓存wlock无效

通常，当一个客户端获取表的WRITE锁时，如果查询结果存在于查询缓存中，则不会阻止其他客户端发出从表读取的语句。将此变量设置为1会导致获取表的WRITE锁，从而使查询缓存中引用该表的任何查询无效。这会迫使其他试图访问该表的客户端在锁定生效时等待。

从MySQL 5.7.20开始，查询缓存已被弃用，并在MySQL 8.0中被删除。弃用包括query_cache_wlock_invalidate。

## query_prealloc_size

> 查询前缀大小

用于语句解析和执行的持久缓冲区的大小（以字节为单位）。在语句之间不会释放此缓冲区。如果您正在运行复杂的查询，较大的query_prealloc_size值可能有助于提高性能，因为它可以减少服务器在查询执行操作期间执行内存分配的需要。您应该意识到，这样做并不一定会完全取消分配；服务器在某些情况下仍然可以分配内存，例如用于与事务或存储程序相关的操作。

## rand_seed1

> 兰特种子1

rand_seed1和rand_seed2变量仅作为会话变量存在，可以设置但不能读取。变量（但不是它们的值）显示在SHOW variables的输出中。

这些变量的目的是支持RAND（）函数的复制。对于调用RAND（）的语句，源将两个值传递给副本，用于为随机数生成器设定种子。复制副本使用这些值来设置会话变量rand_seed1和rand_seed2，以便复制副本上的rand（）生成与源上相同的值。

## rand_seed2

> 兰特种子2

请参阅rand_seed1的说明。

## range_alloc_block_size

> 范围分配块大小

进行范围优化时分配的块的大小（以字节为单位）。

字节号的块大小为1024。在存储系统变量的值之前，MySQL Server会将不是块大小的精确倍数的值四舍五入到块大小的下一个较低倍数。解析器允许平台的最大无符号整数值（对于32位系统为4294967295或232−1，对于64位系统为18446744073709551615或264−1），但实际最大值要低一个块大小。

## range_optimizer_max_mem_size

> 范围优化器最大内存大小

范围优化器的内存消耗限制。值0表示“没有限制”。如果优化器考虑的执行计划使用范围访问方法，但优化器估计此方法所需的内存量将超过限制，则会放弃该计划并考虑其他计划。有关详细信息，请参阅限制内存用于范围优化。

## rbr_exec_mode

> rbr执行模式

供mysqlbinlog内部使用。此变量用于在IDEMPOTENT模式和STRICT模式之间切换服务器。IDEMPOTENT模式会抑制mysqlbinlog生成的BINLOG语句中的重复密钥和未发现密钥错误。当在服务器上重播导致与现有数据冲突的基于行的二进制日志时，此模式非常有用。当您通过向输出中写入以下内容来指定--幂等选项时，mysqlbinlog会设置此模式：

```sql
SET SESSION RBR_EXEC_MODE=IDEMPOTENT;
```

## read_buffer_size

> 读取缓冲区大小

对MyISAM表进行顺序扫描的每个线程为其扫描的每个表分配一个大小（以字节为单位）的缓冲区。如果进行多次顺序扫描，则可能需要增加此值，默认值为131072。此变量的值应该是4KB的倍数。如果将其设置为不是4KB倍数的值，则其值将四舍五入到最接近的4KB倍数。

此选项也用于所有存储引擎的以下上下文：

- 用于缓存临时文件（而非临时表）中的索引，在为ORDER BY排序行时使用。
- 用于大容量插入分区。
- 用于缓存嵌套查询的结果。

read_buffer_size还用于另一种特定于存储引擎的方式：确定memory表的内存块大小。

有关不同操作期间内存使用的更多信息，请参阅第8.12.4.1节“MySQL如何使用内存”。

## read_only

> 只读

如果启用了read_only系统变量，则服务器不允许客户端更新，但具有SUPER权限的用户除外。默认情况下，此变量处于禁用状态。

服务器还支持super_read_only系统变量（默认情况下禁用），该变量具有以下效果：

- 如果启用了super_read_only，则服务器将禁止客户端更新，甚至禁止具有super权限的用户进行更新。
- 将super_read_only设置为ON隐含地强制read_only为ON。
- 将read_only设置为OFF隐含地强制super_read_only为OFF。

即使启用了read_only，服务器也允许执行以下操作：

- 如果服务器是复制副本，则由复制线程执行更新。在复制设置中，只在副本服务器上启用read_only可以确保副本只接受来自源服务器而不是客户端的更新，这一点非常有用。
- ANALYZE TABLE或OPTIMIZE TABLE语句的使用。只读模式的目的是防止更改表结构或内容。分析和优化不属于此类更改。例如，这意味着可以使用mysqlcheck（所有数据库）analyze对只读副本执行一致性检查。
- 使用FLUSH STATUS语句，这些语句总是写入二进制日志。
- 临时表上的操作。
- 插入日志表（mysql.general_log和mysql.slow_log）；请参阅第5.4.1节“选择常规查询日志和慢速查询日志输出目的地”。
- 从MySQL 5.7.16开始，对性能模式表进行更新，如UPDATE或TRUNCATE TABLE操作。

对复制源服务器上只读的更改不会复制到副本服务器。可以在复制副本上设置该值，而与源上的设置无关。

以下条件适用于启用read_only的尝试（包括由于启用super_read_only而导致的隐式尝试）：

- 如果您有任何显式锁（使用LOCK TABLES获取）或有挂起的事务，则尝试失败并发生错误。
- 当其他客户端有任何正在进行的语句、活动的LOCK TABLES WRITE或正在进行的提交时，尝试会被阻止，直到锁被释放，语句和事务结束。当启用read_only的尝试挂起时，其他客户端对表锁或开始事务的请求也会被阻止，直到设置了read_onley。
- 如果存在持有元数据锁的活动事务，则尝试将被阻止，直到这些事务结束。
- 当您持有全局读锁（使用FLUSH TABLES with read lock获取）时，可以启用read_only，因为这不涉及表锁。

## read_rnd_buffer_size

> 读取rnd缓冲区大小

此变量用于从MyISAM表中读取，对于任何存储引擎，用于多范围读取优化。

在执行键排序操作后，按排序顺序从MyISAM表中读取行时，会通过该缓冲区读取行，以避免磁盘查找。参见第8.2.1.14节“按优化排序”。将变量设置为较大的值可以大大提高ORDER BY的性能。但是，这是为每个客户端分配的缓冲区，因此不应将全局变量设置为大值。相反，只从那些需要运行大型查询的客户端中更改会话变量。

有关不同操作期间内存使用的更多信息，请参阅第8.12.4.1节“MySQL如何使用内存”。有关多量程读取优化的信息，请参阅第8.2.1.10节“多量程读取最优化”。

## relay_log

> 继电器日志

## relay_log_basename

> 中继日志基名称

## relay_log_index

> 中继日志索引

## relay_log_info_file

> 中继日志信息文件

## relay_log_info_repository

> 中继日志信息存储库

## relay_log_purge

> 中继日志清除

## relay_log_recovery

> 中继日志恢复

## relay_log_space_limit

> 继电器日志空间限制

## replication_optimize_for_static_plugin_config

> 针对静态插件配置的复制优化

## replication_sender_observe_commit_only

> 复制发送方仅观察提交

## report_host

> 报表主机

## report_password

> 报表密码

## report_port

> 报告端口

## report_user

> 报表用户

## require_secure_transport

> 需要安全运输

是否需要客户端连接到服务器才能使用某种形式的安全传输。启用此变量后，服务器仅允许使用TLS/SSL加密的TCP/IP连接，或使用套接字文件（在Unix上）或共享内存（在Windows上）的连接。服务器拒绝不安全的连接尝试，尝试失败时会出现ER_SECURE_TRANSPORT_REQUIRED错误。

此功能补充了优先考虑的每个帐户SSL要求。例如，如果使用REQUIRE SSL定义帐户，则启用REQUIRE_secure_transport将无法使用该帐户使用Unix套接字文件进行连接。

服务器可能没有可用的安全传输。例如，如果Windows上的服务器在未指定任何SSL证书或密钥文件且已禁用shared_memory系统变量的情况下启动，则不支持安全传输。在这些情况下，尝试在启动时启用require_secure_transport会导致服务器在错误日志中写入一条消息并退出。尝试在运行时启用变量失败，并出现ER_NO_SECURE_TRANSPORTS_CONFIGURED错误。

另请参阅[将加密连接配置为强制连接](https://dev.mysql.com/doc/refman/5.7/en/using-encrypted-connections.html#mandatory-encrypted-connections)。

## rpl_stop_slave_timeout

> rpl停止从属超时

## secure_auth

> 安全身份验证

如果启用了此变量，则服务器会阻止尝试使用密码存储在旧（4.1之前）格式中的帐户的客户端进行连接。启用此变量可以防止所有使用旧格式的密码（从而防止通过网络进行不安全的通信）。

此变量已弃用；期望它在MySQL的未来版本中被删除。它总是处于启用状态，尝试禁用它会产生错误。

如果启用了此变量并且权限表的格式为4.1之前的版本，则服务器启动失败并出现错误。请参阅第6.4.1.3节“从4.1之前版本的密码哈希和mysql_old_Password插件迁移”。

使用4.1之前版本哈希方法的密码不如使用本机密码哈希方法的安全，应避免使用。4.1之前的密码已被弃用，MySQL 5.7.5中删除了对它们的支持。有关帐户升级的说明，请参阅第6.4.1.3节“从4.1之前版本的密码哈希和mysql_old_Password插件迁移”。

## secure_file_priv

> 安全文件priv

此变量用于限制数据导入和导出操作的效果，例如LOAD data和SELECT。。。INTO OUTFILE语句和LOAD_FILE（）函数。这些操作只允许具有FILE权限的用户执行。

secure_file_priv可以如下设置：

- 如果为空，则变量无效。这不是一个安全的设置。
- 如果设置为目录名，则服务器将导入和导出操作限制为仅使用该目录中的文件。目录必须存在；服务器不会创建它。
- 如果设置为NULL，则服务器将禁用导入和导出操作。

默认值是特定于平台的，取决于INSTALL_LAYOUT CMake选项的值，如下表所示。如果从源代码生成，要显式指定默认的secure_file_priv值，请使用INSTALL_secure_file_PRIVDIR CMake选项。

INSTALL_LAYOUT Value| Default secure_file_priv Value
--|--
STANDALONE, WIN |NULL (>= MySQL 5.7.16), empty (< MySQL 5.7.16)
DEB, RPM, SLES, SVR4| /var/lib/mysql-files
Otherwise |mysql-files under the CMAKE_INSTALL_PREFIX value

要设置libmysqld嵌入式服务器的默认secure_file_priv值，请使用INSTALL_secure_file_priv_EMBEDDIR CMake选项。此选项的默认值为NULL。

服务器在启动时检查secure_file_priv的值，如果该值不安全，则会在错误日志中写入警告。如果非NULL值为空，或者该值是数据目录或其子目录，或者是所有用户都可以访问的目录，则认为该值不安全。如果secure_file_priv设置为不存在的路径，则服务器会在错误日志中写入一条错误消息并退出。

## server_id

> 服务器id

## server_id_bits

> 服务器id位

## server_uuid

> 服务器uuid

## session_track_gtids

> 会话跟踪gtid

## session_track_schema

> 会话跟踪模式

控制服务器是否向客户端返回GTID，使客户端能够使用它们来跟踪服务器状态。根据变量值，在执行每个事务结束时，服务器的GTID会被捕获并作为确认的一部分返回给客户端。session_track_gtids的可能值如下：

- OFF：服务器不向客户端返回GTID。这是默认设置。
- OWN_GTID：服务器返回自上次确认以来该客户端在其当前会话中成功提交的所有事务的GTID。通常，这是提交的最后一个事务的单个GTID，但如果单个客户端请求导致多个事务，则服务器会返回一个包含所有相关GTID的GTID集。
- ALL_GTIDS：服务器返回其gtid_executed系统变量的全局值，该值在事务成功提交后读取。除了刚刚提交的事务的GTID外，该GTID集还包括任何客户端在服务器上提交的所有事务，并且可以包括在提交当前被确认的事务之后提交的事务。
  
不能在事务中设置session_track_gtids。

有关会话状态跟踪的更多信息，请参阅[第5.1.15节“客户端会话状态的服务器跟踪”](https://dev.mysql.com/doc/refman/5.7/en/session-state-tracking.html)。

## session_track_state_change

> 会话跟踪状态更改

控制服务器是否跟踪对当前会话状态的更改，并在状态发生更改时通知客户端。可以报告客户端会话状态的这些属性的更改：

- 默认架构（数据库）。
- 系统变量的会话特定值。
- 用户定义的变量。
- 临时表格。
- 准备好的发言。

如果启用了会话状态跟踪器，即使新的属性值与旧的属性值相同，也会为涉及跟踪的会话属性的每个更改发出通知。例如，将用户定义的变量设置为其当前值会导致通知。

session_track_state_change变量仅控制何时发生更改的通知，而不控制更改内容。例如，当设置了默认模式或分配了跟踪会话系统变量，但通知中不包括模式名称或变量值时，会出现状态更改通知。要接收模式名称或会话系统变量值的通知，请分别使用session_track_schema或session_track _system_variables系统变量。

将值分配给session_track_state_change本身不被视为状态更改，也不会报告为状态更改。但是，如果它的名称列在session_track_system_variables的值中，则对它的任何赋值都会导致新值的通知。

有关会话状态跟踪的更多信息，请参阅[第5.1.15节“客户端会话状态的服务器跟踪”](https://dev.mysql.com/doc/refman/5.7/en/session-state-tracking.html)。

## session_track_system_variables

> 会话跟踪系统变量

控制服务器是否跟踪对会话系统变量的分配，并将每个分配变量的名称和值通知客户端。变量值是一个逗号分隔的变量列表，用于跟踪分配。默认情况下，会为time_zone、autocommit、character_set_client、character_set_results和character_set_connection启用通知。（后三个变量是受SET NAMES影响的变量。）

特殊值*使服务器跟踪对所有会话变量的分配。如果给定，则该值必须由其自身指定，而不使用特定的系统变量名。

要禁用会话变量分配通知，请将session_track_system_variables设置为空字符串。

如果启用了会话系统变量跟踪，则即使新值与旧值相同，也会为被跟踪会话变量的所有分配发出通知。

## session_track_transaction_info

> 会话跟踪事务信息

控制服务器是否跟踪当前会话中事务的状态和特征，并通知客户端使这些信息可用。允许这些session_track_transaction_info值：

- OFF：禁用事务状态跟踪。这是默认设置。
- STATE：启用事务状态跟踪，不进行特征跟踪。状态跟踪使客户端能够确定事务是否正在进行中，以及是否可以在不回滚的情况下将其移动到其他会话。
- 特征：启用交易状态跟踪，包括特征跟踪。特征跟踪使客户端能够确定如何在另一个会话中重新启动事务，使其具有与原始会话中相同的特征。以下特征与此相关：

  ```sql
  ISOLATION LEVEL
  READ ONLY
  READ WRITE
  WITH CONSISTENT SNAPSHOT
  ```

为了让客户端安全地将事务重新定位到另一个会话，它不仅必须跟踪事务状态，还必须跟踪事务特征。此外，客户端必须跟踪transaction_inisolation和transaction_read_only系统变量，以正确确定会话默认值。（要跟踪这些变量，请将它们列在session_track_system_variables系统变量的值中。）

## sha256_password_auto_generate_rsa_keys

> sha256密码自动生成rsa密钥

如果服务器是使用OpenSSL编译的，则此变量可用（请参阅第6.3.4节“SSL库相关功能”）。它控制服务器是否在数据目录中自动生成RSA私钥/公钥对文件（如果它们还不存在）。

启动时，如果启用了sha256_password_auto_generate_RSA_keys系统变量，未指定RSA选项，并且数据目录中缺少RSA文件，则服务器会自动在数据目录中生成RSA私钥/公钥对文件。这些文件使通过sha256_password插件验证的帐户能够通过未加密的连接使用RSA进行安全的密码交换；请参阅第6.4.1.5节“SHA-256可插拔身份验证”。

有关RSA文件自动生成的更多信息，包括文件名和特征，请参阅第6.3.3.1节“使用MySQL创建SSL和RSA证书和密钥”

auto_generate_certs系统变量是相关的，但控制使用SSL进行安全连接所需的SSL证书和密钥文件的自动生成。

## sha256_password_private_key_path

> sha256密码私钥路径

如果MySQL是使用OpenSSL编译的，则此变量可用（请参阅第6.3.4节“SSL库相关功能”）。其值是sha256_password身份验证插件的RSA私钥文件的路径名。如果将文件命名为相对路径，则会将其解释为相对于服务器数据目录。文件必须为PEM格式。

因为这个文件存储了一个私钥，所以它的访问模式应该受到限制，这样只有MySQL服务器才能读取它。

有关sha256_password的信息，请参阅[第6.4.1.5节“SHA-256可插拔身份验证”](https://dev.mysql.com/doc/refman/5.7/en/sha256-pluggable-authentication.html)。

## sha256_password_proxy_users

> sha256密码代理用户

此变量控制sha256_password内置身份验证插件是否支持代理用户。除非启用了check_proxy_users系统变量，否则它将无效。有关用户代理的信息，请参阅第6.2.14节“代理用户”。

## sha256_password_public_key_path

> sha256密码公钥路径

如果MySQL是使用OpenSSL编译的，则此变量可用（请参阅第6.3.4节“SSL库相关功能”）。其值是sha256_password身份验证插件的RSA公钥文件的路径名。如果将文件命名为相对路径，则会将其解释为相对于服务器数据目录。文件必须为PEM格式。因为此文件存储公钥，所以副本可以自由分发给客户端用户。（使用RSA密码加密连接到服务器时明确指定公钥的客户端必须使用与服务器使用的公钥相同的公钥。）

## shared_memory

> 共享内存

（仅限Windows。）服务器是否允许共享内存连接。

## shared_memory_base_name

> 共享内存基本名称

（仅限Windows。）用于共享内存连接的共享内存的名称。当在一台物理机器上运行多个MySQL实例时，这很有用。默认名称为MYSQL。该名称区分大小写。

仅当服务器启动时启用了shared_memory系统变量以支持共享内存连接时，此变量才适用。

## show_compatibility_56

> 显示兼容性56

INFORMATION_SCHEMA具有包含系统和状态变量信息的表格（请参阅第24.3.11节“INFORMATION_SCHEMA GLOBAL_VARIABLES和SESSION_VARIABLES表格”和第24.3.10节“INFORMATION_SCHEMA GLOBAL_status和SESSION_status表格”）。从MySQL 5.7.6开始，性能模式还包含系统和状态变量表（参见第25.12.13节“性能模式系统变量表”和第25.12.14节“绩效模式状态变量表”）。性能模式表旨在取代INFORMATION_Schema表，这些表自MySQL 5.7.6起已弃用，并在MySQL 8.0中删除。

有关从INFORMATION_SCHEMA表迁移到性能模式表的建议，请参阅第25.20节“迁移到性能架构系统和状态变量表”。为了帮助迁移，您可以使用show_compatibility_56系统变量，它会影响是否启用MySQL 5.6兼容性，以及information_SCHEMA和Performance SCHEMA表以及show VARIABLES和show status语句如何提供系统和状态变量信息。

show_compatibility_56不推荐使用，因为它的唯一目的是允许控制不推荐使用的系统和状态变量信息源，您可以期望在MySQL的未来版本中删除这些信息源。当这些源被删除后，show_compatibility_56就不再有任何用途，您可以期待它也被删除。

## show_create_table_verbosity

> 显示创建表的详细信息

如果行格式为默认格式，则SHOW CREATE TABLE通常不显示ROW_FORMAT表选项。启用此变量会导致SHOW CREATE TABLE显示ROW_FORMAT，而不管它是否为默认格式。

## show_old_temporals

> 显示旧时态

SHOW CREATE TABLE输出是否包括注释，以标记5.6.4之前版本格式的临时列（不支持小数秒精度的TIME、DATETIME和TIMESTAMP列）。默认情况下，此变量处于禁用状态。如果启用，SHOW CREATE TABLE输出如下所示：

```sql
CREATE TABLE `mytbl` (
  `ts` timestamp /* 5.5 binary format */ NOT NULL DEFAULT CURRENT_TIMESTAMP,
  `dt` datetime /* 5.5 binary format */ DEFAULT NULL,
  `t` time /* 5.5 binary format */ DEFAULT NULL
) DEFAULT CHARSET=latin1
```

信息模式COLUMNS表的COLUMN_TYPE列的输出也受到类似的影响。

此变量已弃用；期望它在MySQL的未来版本中被删除。

## skip_external_locking

> 跳过外部锁定

如果mysqld使用外部锁定（系统锁定），则此选项为OFF，如果禁用了外部锁定，则为ON。这仅影响MyISAM表访问。

此变量由--external locking或--skip external lock选项设置。默认情况下禁用外部锁定。

外部锁定仅影响MyISAM表访问。有关更多信息，包括可使用和不可使用的条件，请参阅[第8.11.5节“外部锁定”](https://dev.mysql.com/doc/refman/5.7/en/external-locking.html)。

## skip_name_resolve

> 跳过名称解析

检查客户端连接时是否解析主机名。如果此变量为OFF，则mysqld在检查客户端连接时解析主机名。如果是ON，则mysqld只使用IP号码；在这种情况下，授权表中的所有主机列值都必须是IP地址。请参阅第5.1.1.2节“DNS查找和主机缓存”。

根据系统的网络配置和帐户的主机值，客户端可能需要使用显式的--Host选项进行连接，例如--Host=127.0.0.1或--Host=：：1。

尝试连接到主机127.0.0.1通常解析为localhost帐户。但是，如果服务器在启用skip_name_resolve的情况下运行，则此操作将失败。如果您计划这样做，请确保存在可以接受连接的帐户。例如，要使用--host=127.0.0.1或--host=：：1以root身份连接，请创建以下帐户：

```sql
CREATE USER 'root'@'127.0.0.1' IDENTIFIED BY 'root-password';
CREATE USER 'root'@'::1' IDENTIFIED BY 'root-password';
```

## skip_networking

> 跳过网络

此变量控制服务器是否允许TCP/IP连接。默认情况下，它被禁用（允许TCP连接）。如果启用，服务器只允许本地（非TCP/IP）连接，并且必须使用命名管道或共享内存（在Windows上）或Unix套接字文件（在Unix上）与mysqld进行所有交互。强烈建议仅允许使用本地客户端的系统使用此选项。请参阅第5.1.1.2节“DNS查找和主机缓存”。

## skip_show_database

> 跳过显示数据库

如果没有SHOW DATABASES权限，这将阻止用户使用SHOW DATABASE语句。如果您担心用户能够看到属于其他用户的数据库，这可以提高安全性。其效果取决于SHOW DATABASES权限：如果变量值为on，则SHOW database语句仅允许具有SHOW DATABASES权限的用户使用，并且该语句显示所有数据库名称。如果该值为OFF，则允许所有用户使用SHOW DATABASES，但仅显示用户具有SHOW DATABASE或其他特权的那些数据库的名称。

由于全局权限被视为所有数据库的权限，因此任何全局权限都允许用户使用SHOW databases或通过检查INFORMATION_SCHEMA SCHEMAT表来查看所有数据库名称。

## slave_allow_batching

> 从允许批处理

## slave_checkpoint_group

> 从属检查点组

## slave_checkpoint_period

> 从检查点周期

## slave_compressed_protocol

> 从压缩协议

## slave_exec_mode

> 从执行模式

## slave_load_tmpdir

> 从负载tmpdir

## slave_max_allowed_packet

> 从设备允许的最大数据包

## slave_net_timeout

> 从网超时

## slave_parallel_type

> 从并行型

## slave_parallel_workers

> 奴隶平行工人

## slave_pending_jobs_size_max

> 从属挂起作业最大大小

## slave_preserve_commit_order

> 从保留提交顺序

## slave_rows_search_algorithms

> 从行搜索算法

## slave_skip_errors

> 从属跳过错误

## slave_sql_verify_checksum

> 从sql验证校验和

## slave_transaction_retries

> 从属事务重试次数

## slave_type_conversions

> 从类型转换

## slow_launch_time

> 慢速启动时间

如果创建线程的时间超过这几秒，则服务器会递增Slow_launch_threads状态变量。

## slow_query_log

> 慢速查询日志

是否启用慢速查询日志。该值可以为0（或OFF）以禁用日志，也可以为1（或ON）以启用日志。日志输出的目的地由log_output系统变量控制；如果该值为NONE，则即使启用了日志，也不会写入任何日志条目。

“慢速”由long_query_time变量的值决定。请参阅[第5.4.5节“慢速查询日志”](https://dev.mysql.com/doc/refman/5.7/en/slow-query-log.html)。

## slow_query_log_file

> 慢速查询日志文件

慢速查询日志文件的名称。默认值为host_name-slow.log，但可以使用--slow_query_log_file选项更改初始值。

## socket

在Unix平台上，此变量是用于本地客户端连接的套接字文件的名称。默认为/tmp/mysql.sock。（对于某些分发格式，目录可能不同，例如用于RPM的/var/lib/mysql。）

在Windows上，此变量是用于本地客户端连接的命名管道的名称。默认值为MySQL（不区分大小写）。

## sort_buffer_size

> 排序缓冲区大小

每个必须执行排序的会话都会分配一个此大小的缓冲区。sort_buffer_size不特定于任何存储引擎，而是以通用方式应用于优化。sort_buffer_size值至少必须足够大，以便在排序缓冲区中容纳十五个元组。此外，增加max_sort_length的值可能需要增加sort_buffer_size的值。有关更多信息，请参阅第8.2.1.14节“ORDER BY Optimization”

如果在SHOW GLOBAL STATUS输出中每秒看到许多Sort_merge_passes，则可以考虑增加Sort_buffer_size值以加快ORDER BY或GROUP BY操作，这些操作无法通过查询优化或改进索引来改进。

优化器试图计算出需要多少空间，但可以分配更多的空间，达到极限。将其全局设置为大于所需大小会减慢大多数排序查询的速度。最好将其作为会话设置来增加，并且仅适用于需要更大大小的会话。在Linux上，有256KB和2MB的阈值，较大的值可能会显著降低内存分配速度，因此您应该考虑保持在其中一个值以下。尝试为您的工作量找到最佳价值。请参阅B.3.3.5节“MySQL存储临时文件的位置”。

sort_buffer_size的最大允许设置为4GB−1。64位平台允许使用更大的值（64位Windows除外，对于64位Windows，较大的值会截断为4GB−1并发出警告）。

## sql_auto_is_null

> sql auto为null

如果启用了此变量，那么在成功插入自动生成的AUTO_INCREMENT值的语句之后，您可以通过发出以下形式的语句来找到该值：

```sql
SELECT * FROM tbl_name WHERE auto_col IS NULL
```

如果语句返回一行，则返回的值与调用LAST_INSERT_ID（）函数时的值相同。有关详细信息，包括多行插入后的返回值，请参阅第12.15节“信息函数”。如果没有成功插入AUTO_INCREMENT值，SELECT语句将不返回任何行。

某些ODBC程序（如Access）使用通过IS NULL比较检索AUTO_INCREMENT值的行为。请参阅获取自动增量值。可以通过将sql_auto_is_null设置为OFF来禁用此行为。

sql_auto_is_null的默认值为OFF。

## sql_big_selects

> sql大选择

如果设置为OFF，MySQL将中止可能需要很长时间才能执行的SELECT语句（即优化器估计检查的行数超过max_join_size值的语句）。当发布了不可取的WHERE语句时，这很有用。新连接的默认值是ON，它允许所有SELECT语句。

如果将max_join_size系统变量设置为DEFAULT以外的值，则sql_big_selects将设置为OFF。

## sql_buffer_result

> sql缓冲区结果

如果启用，sql_buffer_result将强制SELECT语句的结果放入临时表中。这有助于MySQL尽早释放表锁，并且在需要很长时间才能将结果发送到客户端的情况下，这是有益的。默认值为OFF。

## sql_log_bin

> sql日志箱

此变量控制当前会话是否禁用对常规查询日志的日志记录（假设启用了常规查询日志本身）。默认值为OFF（即启用日志记录）。要禁用或启用当前会话的常规查询日志记录，请将会话sql_log_off变量设置为ON或off。

设置此系统变量的会话值是一项受限制的操作。会话用户必须具有足够的权限来设置受限制的会话变量。参见第5.1.8.1节“系统变量权限”。

## sql_log_off

> sql注销

## sql_mode

> sql模式

当前服务器SQL模式，可以动态设置。有关详细信息，请参阅[第5.1.10节“服务器SQL模式”](https://dev.mysql.com/doc/refman/5.7/en/sql-mode.html)。

## sql_notes

> sql注释

如果已启用（默认设置），则“注释”级别的诊断将递增warning_count，服务器将记录它们。如果禁用，请注意诊断不会增加warning_count，服务器也不会记录它们。mysqldump包含禁用此变量的输出，以便重新加载转储文件不会对不影响重新加载操作完整性的事件产生警告。

## sql_quote_show_create

> sql报价显示创建

如果启用（默认设置），服务器会引用SHOW CREATE TABLE和SHOW CREATE DATABASE语句的标识符。如果禁用，则禁用引用。默认情况下启用此选项，以便复制适用于需要引用的标识符。请参阅第13.7.7.10节“SHOW CREATE TABLE语句”和第13.7.5.6节“SHOW CREATE DATABASE语句”。

## sql_safe_updates

> sql安全更新

如果启用了此变量，则在WHERE子句或LIMIT子句中不使用键的UPDATE和DELETE语句将产生错误。这样就可以捕获键使用不正确的UPDATE和DELETE语句，这可能会更改或删除大量行。默认值为OFF。

对于mysql客户端，可以使用--safe_updates选项启用sql_safe_updates。有关详细信息，请参阅使用安全更新模式（--Safe Updates）。

## sql_select_limit

> sql选择限制

从SELECT语句返回的最大行数。有关详细信息，请参阅[使用安全更新模式（--Safe Updates）](https://dev.mysql.com/doc/refman/5.7/en/mysql-tips.html#safe-updates)。

新连接的默认值是服务器允许的每个表的最大行数。典型的默认值为（232）−1或（264）−1。如果更改了限制，则可以通过指定default值来恢复默认值。

如果SELECT有LIMIT子句，则LIMIT优先于sql_SELECT_LIMIT的值。

## sql_slave_skip_counter

> sql从跳过计数器

## sql_warnings

> sql警告

此变量控制单行INSERT语句在出现警告时是否生成信息字符串。默认值为OFF。将该值设置为ON可生成信息字符串。

## ssl_ca

> ssl ca

PEM格式的证书颁发机构（CA）证书文件的路径名。该文件包含受信任的SSL证书颁发机构的列表。

## ssl_capath

> ssl容量

包含PEM格式的受信任SSL证书颁发机构（CA）证书文件的目录的路径名。对该功能的支持取决于用于编译MySQL的SSL库；请参阅第6.3.4节“SSL库相关功能”。

## ssl_cert

> ssl证书

PEM格式的服务器SSL公钥证书文件的路径名。

如果服务器启动时将ssl_cert设置为使用任何受限密码或密码类别的证书，则服务器启动时禁用对加密连接的支持。有关密码限制的信息，请参阅连接密码配置。

## ssl_cipher

> ssl密码

用于连接加密的允许密码的列表。如果列表中不支持密码，则加密连接将不起作用。

为了实现最大的可移植性，密码列表应该是一个或多个密码名称的列表，用冒号分隔。OpenSSL和yaSSL都能理解这种格式。以下示例显示了两个用冒号分隔的密码名称：

```sql
[mysqld]
ssl_cipher="DHE-RSA-AES128-GCM-SHA256:AES128-SHA"
```

OpenSSL支持更灵活的语法来指定密码，如OpenSSL文档中所述<https://www.openssl.org/docs/manmaster/man1/openssl-ciphers.html.yaSSL没有，所以对于使用yaSSL编译的MySQL分发版，尝试使用该扩展语法失败。>

有关MySQL支持哪些加密密码的信息，请参阅[第6.3.2节“加密连接TLS协议和密码”](https://dev.mysql.com/doc/refman/5.7/en/encrypted-connection-protocols-ciphers.html)。

## ssl_crl

> ssl crl

包含PEM格式的证书吊销列表的文件的路径名。对吊销列表功能的支持取决于用于编译MySQL的SSL库。请参阅第6.3.4节“SSL库相关功能”。

## ssl_crlpath

> ssl crlpath

包含PEM格式的证书吊销列表文件的目录的路径。对吊销列表功能的支持取决于用于编译MySQL的SSL库。请参阅第6.3.4节“SSL库相关功能”。

## ssl_key

> ssl密钥

PEM格式的服务器SSL私钥文件的路径名。为了提高安全性，请使用RSA密钥大小至少为2048位的证书。

如果密钥文件受密码短语保护，则服务器会提示用户输入密码短语。密码必须以交互方式提供；它不能存储在文件中。如果密码短语不正确，程序将继续运行，就像无法读取密钥一样。

## stored_program_cache

> 存储程序缓存

设置每个连接的缓存存储例程数的软上限。此变量的值是根据MySQL Server分别为存储过程和存储函数维护的两个缓存中的每个缓存中存储例程的数量来指定的。

每当执行存储的例程时，在解析例程中的第一个或顶级语句之前检查该缓存大小；如果同一类型的例程（执行所依据的存储过程或存储函数）的数量超过该变量指定的限制，则会刷新相应的缓存，并释放先前为缓存对象分配的内存。这允许安全地刷新缓存，即使存储的例程之间存在依赖关系。

## super_read_only

> 超级只读

如果启用了read_only系统变量，则服务器不允许客户端更新，但具有SUPER权限的用户除外。如果还启用了super_read_only系统变量，则服务器甚至禁止具有super的用户进行客户端更新。有关只读模式的描述以及read_only和super_read_only如何交互的信息，请参阅read_onley系统变量的描述。

启用super_read_only时阻止的客户端更新包括不一定显示为更新的操作，如CREATE FUNCTION（安装可加载函数）和install PLUGIN。这些操作是被禁止的，因为它们涉及到对mysql系统数据库中的表的更改。

仅在复制源服务器上对super_read_only所做的更改不会复制到副本服务器。可以在复制副本上设置该值，而与源上的设置无关。

## sync_binlog

> 同步binlog

## sync_frm

> 同步frm

如果此变量设置为1，则在创建任何非临时表时，其.frm文件都会同步到磁盘（使用fdatasync（））。这速度较慢，但在发生碰撞时更安全。默认值为1。

此变量在MySQL 5.7中已弃用，在MySQL 8.0中已删除（当.frm文件过时时）。

## sync_master_info

> 同步主信息

## sync_relay_log

> 同步中继日志

## sync_relay_log_info

> 同步中继日志信息

## system_time_zone

> 系统时区

服务器系统时区。当服务器开始执行时，它会从机器默认值继承时区设置，该设置可能会被用于运行服务器或启动脚本的帐户的环境修改。该值用于设置system_time_zone。要显式指定系统时区，请设置TZ环境变量或使用mysqld_safe脚本的--timezone选项。

system_time_zone变量与time_zone不同。尽管它们可能具有相同的值，但后一个变量用于初始化连接的每个客户端的时区。请参阅第5.1.13节“MySQL Server时区支持”。

## table_definition_cache

> 表定义缓存

可以存储在表定义缓存中的表定义数（来自.frm文件）。如果使用大量表，可以创建大型表定义缓存以加快打开表的速度。与普通表缓存不同，表定义缓存占用的空间较小，并且不使用文件描述符。最小值为400。默认值基于以下公式，上限为2000：

```sql
400 + (table_open_cache / 2)
```

对于InnoDB，table_definition_cache设置充当InnoDB数据字典缓存中表实例数量和每次可打开的每个表表空间的文件数量的软限制。

如果InnoDB数据字典缓存中的表实例数量超过table_definition_cache限制，LRU机制开始标记表实例以进行驱逐，并最终将其从InnoDB数据词典缓存中删除。具有缓存元数据的打开表的数量可能高于table_definition_cache限制，这是由于具有外键关系的表实例不在LRU列表中。

一次可以打开的每个表表空间的文件数受table_definition_cache和innodb_open_files设置的限制。如果同时设置了两个变量，则使用最高设置。如果两个变量都未设置，则使用默认值较高的table_definition_cache设置。如果打开的表空间的数量超过table_definition_cache或innodb_open_files定义的限制，则LRU机制在LRU列表中搜索已完全刷新且当前未扩展的表空间文件。每次打开新的表空间时都会执行此过程。只有不活动的表空间是关闭的。

## table_open_cache

> 表打开缓存

所有线程打开的表数。增加这个值会增加mysqld所需的文件描述符的数量。此变量的有效值是open_files_limit的有效值-10-max_connections/2的有效值和400中的较大值；那就是

```sql
MAX(
    (open_files_limit - 10 - max_connections) / 2,
    400
   )
```

您可以通过检查Opened_tables状态变量来检查是否需要增加表缓存。如果Opened_tables的值很大，并且不经常使用FLUSH tables（这只是强制关闭并重新打开所有表），则应增加table_open_cache变量的值。有关表缓存的更多信息，请参阅第8.4.3.1节“MySQL如何打开和关闭表”。

## table_open_cache_instances

> 表打开缓存实例

打开的表缓存实例的数量。为了通过减少会话之间的争用来提高可扩展性，可以将开放表缓存划分为几个较小的缓存实例，大小为table_open_cache/table_open_cachi_instances。会话只需要锁定一个实例，就可以为DML语句访问它。这样可以在实例之间分割缓存访问，从而在有许多会话访问表时，允许使用缓存的操作具有更高的性能。（DDL语句仍然需要对整个缓存进行锁定，但此类语句的频率远低于DML语句。）

对于常规使用16个或更多核心的系统，建议使用8或16的值。但是，如果表上有许多导致高内存负载的大型触发器，则table_open_cache_instances的默认设置可能会导致过度使用内存。在这种情况下，将table_open_cache_instances设置为1以限制内存使用可能会有所帮助。

## thread_cache_size

> 线程缓存大小

服务器应该缓存多少个线程以供重用。当客户端断开连接时，如果缓存中的线程少于thread_cache_size，则会将客户端的线程放入缓存中。如果可能的话，通过重用从缓存中获取的线程来满足对线程的请求，并且只有当缓存为空时才创建新的线程。如果有很多新连接，可以增加此变量以提高性能。通常，如果您有一个好的线程实现，这不会显著提高性能。但是，如果服务器每秒看到数百个连接，通常应该将thread_cache_size设置得足够高，以便大多数新连接使用缓存的线程。通过检查Connections和Threads_created状态变量之间的差异，您可以了解线程缓存的效率。有关详细信息，请参阅第5.1.9节“服务器状态变量”。

默认值基于以下公式，上限为100：

```sql
8 + (max_connections / 100)
```

此变量对嵌入式服务器（libmysqld）没有影响，并且从MySQL 5.7.2起，在嵌入式服务器中不再可见。

## thread_handling

> 线程处理

服务器用于连接线程的线程处理模型。允许的值是无线程（服务器使用单个线程来处理一个连接）、每个连接一个线程（服务器用一个线程来处理每个客户端连接）和动态加载（由线程池插件初始化时设置）。没有线程可用于Linux下的调试；请参阅第5.8节“调试MySQL”。

此变量对嵌入式服务器（libmysqld）没有影响，并且从MySQL 5.7.2起，在嵌入式服务器中不再可见。

## thread_pool_algorithm

> 线程池算法

此变量控制线程池插件使用的算法：

- 值为0（默认值）使用保守的低并发算法，该算法经过了最充分的测试，并且可以产生非常好的结果。
- 值为1会增加并发性，并使用更激进的算法，该算法有时在最佳线程数上的性能会提高5–10%，但随着连接数量的增加，性能会降低。它的使用应被视为实验性的，不受支持。

仅当启用线程池插件时，此变量才可用。请参阅[第5.5.3节“MySQL企业线程池”](https://dev.mysql.com/doc/refman/5.7/en/thread-pool.html)。

## thread_pool_high_priority_connection

> 线程池高优先级连接

此变量影响执行前新语句的排队。如果值为0（默认值为false），则语句队列同时使用低优先级和高优先级队列。如果值为1（true），则排队的语句总是转到高优先级队列。

## thread_pool_max_unused_threads

> 线程池最大未使用线程数

线程池中允许的最大未使用线程数。这个变量可以限制睡眠线程使用的内存量。

值为0（默认值）意味着睡眠线程的数量没有限制。其中N大于0的值N表示1个使用者线程和N−1个保留线程。在这种情况下，如果线程已准备好睡眠，但睡眠线程的数量已经达到最大值，则该线程将退出，而不是进入睡眠状态。

睡眠线程要么作为使用者线程睡眠，要么作为保留线程睡眠。线程池允许一个线程在睡眠时作为使用者线程。如果一个线程进入睡眠状态，并且没有现有的使用者线程，那么它将作为使用者线程睡眠。当一个线程必须被唤醒时，如果有使用者线程，就会选择一个使用者线程。只有当没有要唤醒的使用者线程时，才会选择保留线程。

## thread_pool_prio_kickup_timert

> 线程池prio启动计时器

此变量影响在低优先级队列中等待执行的语句。该值是等待语句移动到高优先级队列之前的毫秒数。默认值为1000（1秒）。

## thread_pool_size

> 线程池大小

线程池中线程组的数目。这是控制线程池性能的最重要的参数。它影响可以同时执行的语句数。如果指定了超出允许值范围的值，则不会加载线程池插件，服务器会在错误日志中写入消息。

## thread_pool_stall_limit

> 线程池暂停限制

此变量影响执行语句。该值是一条语句在开始执行后，在被定义为停滞之前必须完成的时间量，此时线程池允许线程组开始执行另一条语句。该值以10毫秒为单位进行测量，因此默认值6表示60毫秒。短等待值允许线程更快地启动。短值对于避免死锁情况也更好。长等待值对于包含长时间运行语句的工作负载非常有用，以避免在执行当前语句时启动过多的新语句。

## thread_stack

> 线程堆栈

每个线程的堆栈大小。默认值足够大，可以正常操作。如果线程堆栈大小太小，则会限制服务器可以处理的SQL语句的复杂性、存储过程的递归深度以及其他消耗内存的操作。

## time_format

> 时间格式

此变量未使用。它已被弃用，并在MySQL 8.0中被删除。

## time_zone

> 时区

当前时区。此变量用于初始化连接的每个客户端的时区。默认情况下，它的初始值为“SYSTEM”（意思是“使用SYSTEM_time_zone的值”）。该值可以在服务器启动时使用--default时区选项显式指定。请参阅第5.1.13节“MySQL Server时区支持”。

如果设置为SYSTEM，则每个需要时区计算的MySQL函数调用都会进行系统库调用，以确定当前系统时区。此调用可能受到全局互斥的保护，从而导致争用。

## timestamp

> 时间戳

设置此客户端的时间。如果您使用二进制日志来恢复行，则使用它来获取原始时间戳。timestamp_value应该是Unix epoch时间戳（类似Unix_timestamp（）返回的值，而不是YYYY-MM-DD hh:MM:ss格式的值）或DEFAULT。

将时间戳设置为常数值会使其保留该值，直到再次更改为止。将时间戳设置为DEFAULT会使其值为访问时的当前日期和时间。最大值对应于'2038-01-19 03:14:07'UTC，与TIMESTAMP数据类型相同。

时间戳是DOUBLE而不是BIGINT，因为它的值包括微秒部分。

SET时间戳会影响NOW（）返回的值，但不会影响SYSDATE（）。这意味着二进制日志中的时间戳设置对SYSDATE（）的调用没有影响。服务器可以使用--sysdate is now选项启动，以使sysdate（）成为now（）的同义词，在这种情况下，SET时间戳会影响这两个函数。

## tls_version

> tls版本

服务器允许哪些协议用于加密连接。该值是一个逗号分隔的列表，包含一个或多个协议版本。可以为此变量命名的协议取决于用于编译MySQL的SSL库。应选择允许的协议，以免在列表中留下“漏洞”。有关详细信息，请参阅第6.3.2节“加密连接TLS协议和密码”。

从MySQL 5.7.35开始，TLSv1和TLSv1.1连接协议已被弃用，对它们的支持可能会在未来版本的MySQL中删除。请参阅不推荐的TLS协议。

## tmp_table_size

> tmp表大小

内存中内部临时表的最大大小。此变量不适用于用户创建的MEMORY表。

实际限制是tmp_table_size和max_heap_table_size中较小的一个。当内存中的临时表超过限制时，MySQL会自动将其转换为磁盘上的临时表。internal_tmp_disk_storage_engine选项定义用于磁盘上临时表的存储引擎。

如果执行了许多高级GROUP BY查询并且有大量内存，请增加tmp_table_size的值（如有必要，还可以增加max_heap_table_size）。

通过比较created_tmp_disk_tables和created_tmp_tables的值，可以将创建的内部磁盘临时表的数量与创建的内部临时表的总数进行比较。

另请参见[第8.4.4节“MySQL中的内部临时表使用”](https://dev.mysql.com/doc/refman/5.7/en/internal-temporary-tables.html)。

## tmpdir

> tmpdir

用于创建临时文件的目录的路径。如果您的默认/tmp目录所在的分区太小，无法容纳临时表，那么这可能会很有用。此变量可以设置为以循环方式使用的几个路径的列表。路径应在Unix上用冒号字符（：）分隔，在Windows上用分号字符（；）分隔。

tmpdir可以是一个非永久位置，例如基于内存的文件系统上的目录，或者在服务器主机重新启动时清除的目录。如果MySQL服务器充当副本，并且您正在使用tmpdir的非永久位置，请考虑使用slave_load_tmpdir变量为副本设置一个不同的临时目录。对于复制副本，用于复制LOAD DATA语句的临时文件存储在此目录中，因此有了一个永久位置，它们可以在机器重新启动后存活下来，尽管如果临时文件已被删除，则复制现在可以在重新启动后继续。

有关临时文件存储位置的更多信息，请参阅[B.3.3.5节“MySQL存储临时文件的位置”](https://dev.mysql.com/doc/refman/5.7/en/temporary-files.html)。

## transaction_alloc_block_size

> 事务分配块大小

需要内存的每个事务内存池增加的字节数。请参阅transaction_precalloc_size的说明。

## transaction_allow_batching

> 事务允许批处理

## transaction_isolation

> 事务隔离

|有效值
|-- |
READ-UNCOMMITTED 已读未提交
READ-COMMITTED 已读提交
REPEATABLE-READ 可重复读取
SERIALIZABLE 可序列化的

事务隔离级别。默认值为REPEATABLE-READ。

事务隔离级别有三个作用域：全局、会话和下一个事务。这三个范围的实现导致了一些非标准的隔离级别赋值语义，如后面所述。

要在启动时设置全局事务隔离级别，请使用--transaction isolation-server选项。

在运行时，可以使用set语句直接设置隔离级别，为transaction_instance系统变量赋值，也可以使用set transaction语句间接设置隔离级别。如果直接将transaction_sisolation设置为包含空格的隔离级别名称，则该名称应括在引号内，空格由短划线代替。例如，使用此SET语句设置全局值：

```sql
SET GLOBAL transaction_isolation = 'READ-COMMITTED';
```

设置全局事务隔离值可设置所有后续会话的隔离级别。现有会话不受影响。

要设置会话或下一级transaction_instance值，请使用set语句。对于大多数会话系统变量，这些语句是设置值的等效方法：

```sql
SET @@SESSION.var_name = value;
SET SESSION var_name = value;
SET var_name = value;
SET @@var_name = value;
```

如前所述，除了全局作用域和会话作用域之外，事务隔离级别还有下一个事务作用域。为了能够设置下一个事务作用域，用于分配会话系统变量值的set语法具有transaction_instance的非标准语义：

- 要设置会话隔离级别，请使用以下任意语法：

  ```sql
  SET @@SESSION.transaction_isolation = value;
  SET SESSION transaction_isolation = value;
  SET transaction_isolation = value;
  ```

  对于这些语法中的每一种，都应用以下语义：
  - 为会话中执行的所有后续事务设置隔离级别。
  - 交易中允许，但不影响当前正在进行的交易。
  - 对应于SET SESSION TRANSACTION ISOLATION LEVEL（使用SESSION关键字）。
- 要设置下一个事务隔离级别，请使用以下语法：

  ```sql
  SET @@transaction_isolation = value;
  ```

  对于该语法，以下语义适用：
  - 仅为会话中执行的下一个单个事务设置隔离级别。
  - 后续事务将恢复到会话隔离级别。
  - 对应于SET TRANSACTION ISOLATION LEVEL（不带SESSION关键字）。

有关SET TRANSACTION及其与TRANSACTION_instance系统变量的关系的更多信息，请参阅[第13.3.6节“SET TRANSACTION语句”。](https://dev.mysql.com/doc/refman/5.7/en/set-transaction.html)

## transaction_prealloc_size

> 事务预分配大小

有一个每个事务的内存池，各种与事务相关的分配从中获取内存。池的初始大小（以字节为单位）为transaction_precalloc_size。对于由于可用内存不足而无法从池中满足的每个分配，池将增加transaction_alloc_block_size字节。当事务结束时，池将被截断为transaction_prealloc_size字节。

通过使transaction_prealloc_size足够大以包含单个事务中的所有语句，可以避免多次malloc（）调用。

## transaction_read_only

> 事务只读

事务访问模式。该值可以是OFF（读/写；默认值）或ON（只读）。

事务访问模式有三个作用域：全局、会话和下一个事务。这种三范围的实现导致了一些非标准的访问模式分配语义，如后面所述。

要在启动时设置全局事务访问模式，请使用--transaction只读服务器选项。

在运行时，可以直接使用set语句为transaction_read_only系统变量赋值，也可以间接使用set transaction语句设置访问模式。例如，使用此SET语句设置全局值：

```sql
SET GLOBAL transaction_read_only = ON;
```

设置全局transaction_read_only值可设置所有后续会话的访问模式。现有会话不受影响。

要设置会话或下一级transaction_read_only值，请使用set语句。对于大多数会话系统变量，这些语句是设置值的等效方法：

```sql
SET @@SESSION.var_name = value;
SET SESSION var_name = value;
SET var_name = value;
SET @@var_name = value;
```

如前所述，除了全局作用域和会话作用域之外，事务访问模式还有下一个事务作用域。为了能够设置下一个事务范围，用于分配会话系统变量值的set语法对于transaction_read_only具有非标准语义，

- 要设置会话访问模式，请使用以下任意语法：

  ```sql
  SET @@SESSION.transaction_read_only = value;
  SET SESSION transaction_read_only = value;
  SET transaction_read_only = value;
  ```

  对于这些语法中的每一种，都应用以下语义：

  - 设置会话中执行的所有后续事务的访问模式。
  - 交易中允许，但不影响当前正在进行的交易。
  - 如果在事务之间执行，则覆盖设置下一个事务访问模式的任何先前语句。
  - 对应于SET SESSION TRANSACTION｛READ WRITE | READ ONLY｝（带有SESSION关键字）。

- 要设置下一个事务访问模式，请使用以下语法：

  ```sql
  SET @@transaction_read_only = value;
  ```

  对于该语法，以下语义适用：

  - 仅为会话中执行的下一个单个事务设置访问模式。
  - 后续事务将恢复到会话访问模式。
  - 不允许在 transactions 之内。
  - 对应于SET TRANSACTION｛READ WRITE | READ ONLY｝（不带SESSION关键字）。
  
有关SET TRANSACTION及其与TRANSACTION_read_only系统变量的关系的更多信息，请参阅第13.3.6节“SET TRANSACTIONStatement”。

transaction_read_only是在MySQL 5.7.20中添加的，作为tx_read_oonly的同义词，现在已弃用，并在MySQL 8.0中删除。应将应用程序调整为仅使用transaction_read_only，而不是仅使用tx_read_only。

## transaction_write_set_extraction

> 事务写入集提取

## tx_isolation

> tx隔离

默认的事务隔离级别。默认为REPEATABLE-READ。

transaction_insolation是在MySQL 5.7.20中添加的，作为tx_isolation的同义词，现在已弃用，并在MySQL 8.0中删除。应调整应用程序，使其优先使用transaction_seilation而不是tx_isolation。有关详细信息，请参阅transaction_instance的说明。

## tx_read_only

> tx只读

默认事务访问模式。该值可以是OFF（读/写，默认值）或ON（只读）。

transaction_read_only是在MySQL 5.7.20中添加的，作为tx_read_oonly的同义词，现在已弃用，并在MySQL 8.0中删除。应将应用程序调整为仅使用transaction_read_only，而不是仅使用tx_read_only。有关详细信息，请参阅transaction_read_only的说明。

## unique_checks

> 唯一的检查

如果设置为1（默认值），将执行InnoDB表中二级索引的唯一性检查。如果设置为0，则允许存储引擎假定输入数据中不存在重复的密钥。如果您确信您的数据不包含唯一性冲突，则可以将其设置为0，以加快向InnoDB导入大表的速度。

将此变量设置为0不需要存储引擎忽略重复的密钥。发动机仍然可以检查它们，如果检测到它们，则可以发出重复的钥匙错误。

## updatable_views_with_limit

> 带限制的可更新视图

如果update语句包含LIMIT子句，则此变量控制当视图不包含基础表中定义的主键的所有列时，是否可以对视图进行更新。（这种更新通常由GUI工具生成。）更新是update或DELETE语句。这里的主键是指Primary key或UNIQUE索引，其中任何列都不能包含NULL。

变量可以有两个值：

- 1或YES：仅发出警告（而不是错误消息）。这是默认值。
- 0或否：禁止更新。

## version

> 版本

服务器的版本号。该值还可能包括指示服务器构建或配置信息的后缀-log表示启用了一个或多个常规日志、慢速查询日志或二进制日志-debug表示服务器是在启用调试支持的情况下生成的。

## version_comment

> 版本注释

CMake配置程序具有COMPILATION_COMMENT选项，该选项允许在构建MySQL时指定注释。此变量包含该注释的值。请参阅第2.8.7节“MySQL源配置选项”。

## version_compile_machine

> 版本编译机

服务器二进制文件的类型。

## version_compile_os

> 版本编译操作系统

MySQL构建所基于的操作系统的类型。

## wait_timeout

> 等待超时

服务器在关闭非交互连接之前等待活动的秒数。

在线程启动时，会话wait_timeout值根据客户端的类型（由指向mysql_real_connect（）的client_interactive连接选项定义）从全局wait_timeout值或全局interactive_timeout值初始化。另请参见interactive_timeout。

## warning_count

> 警告计数

生成消息的最后一条语句所产生的错误、警告和注释的数量。此变量是只读的。参见第13.7.5.40节“显示警告声明”。
