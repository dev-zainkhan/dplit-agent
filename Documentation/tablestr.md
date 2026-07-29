### `Attendance_CarPal`, `Attendance_MM`, `Attendance_NatJan`
| Column Name | Data Type |
| --- | --- |
| `EmployeeName` | `varchar(100)` |
| `Month` | `date` |
| `AvgAttendanceHours` | `decimal(5,2)` |
| `WFODays` | `int` |
| `WFHDays` | `int` |
| `WFO_Percentage` | `decimal(5,2)` |
| `WFH_Percentage` | `decimal(5,2)` |

### `Client_PO_Feedback_CarPal`, `Client_PO_Feedback_MM`, `Client_PO_Feedback_nGage`
| Column Name | Data Type |
| --- | --- |
| `sprint_name` | `text` |
| `sprint_start_date` | `datetime` |
| `sprint_end_date` | `datetime` |
| `task_name` | `text` |
| `rating` | `int` |
| `comment` | `text` |
| `type` | `text` |
| `participants` | `text` | 

### `Client_PO_Feedback_NatJan`
| Column Name | Data Type |
| --- | --- |
| `sprint_name` | `text` |
| `sprint_start_date` | `datetime` |
| `sprint_end_date` | `datetime` |
| `task_name` | `text` |
| `rating` | `decimal(3,1)` |
| `comment` | `text` |
| `type` | `text` |
| `participants` | `text` |
| `requested_from` | `text` |

### `Releases_CarPal`, `Releases_MM`, `Releases_NatJan`
| Column Name | Data Type |
| --- | --- |
| `Release Name` | `varchar(255)` |
| `Release Date` | `date` |

### `Team_Repository_Analytics_Cursor_CarPal`, `Team_Repository_Analytics_Cursor_MM`
| Column Name | Data Type |
| --- | --- |
| `id` | `bigint` |
| `repo_name` | `varchar(255)` |
| `total_commits` | `int` |
| `total_lines_added` | `int` |
| `total_lines_deleted` | `int` |
| `ai_lines_added` | `int` |
| `ai_lines_deleted` | `int` |
| `ai_impact_percentage` | `decimal(6,2)` |
| `tab_lines_added` | `int` |
| `tab_lines_deleted` | `int` |
| `composer_lines_added` | `int` |
| `composer_lines_deleted` | `int` |
| `non_ai_lines_added` | `int` |
| `non_ai_lines_deleted` | `int` |
| `report_start_date` | `date` |
| `report_end_date` | `date` |
| `source_file` | `varchar(255)` |
| `created_at` | `timestamp` |
| `sprint` | `varchar(100)` |

### `Team_Repository_Analytics_Cursor_nGage`
| Column Name | Data Type |
| --- | --- |
| `id` | `bigint` |
| `repo_name` | `varchar(255)` |
| `total_commits` | `int` |
| `total_lines_added` | `int` |
| `total_lines_deleted` | `int` |
| `ai_lines_added` | `int` |
| `ai_lines_deleted` | `int` |
| `ai_impact_percentage` | `decimal(6,2)` |
| `tab_lines_added` | `int` |
| `tab_lines_deleted` | `int` |
| `composer_lines_added` | `int` |
| `composer_lines_deleted` | `int` |
| `non_ai_lines_added` | `int` |
| `non_ai_lines_deleted` | `int` |
| `sprint` | `int` |
| `report_start_date` | `date` |
| `report_end_date` | `date` |

### `User_Leaderboard_CarPal`, `User_Leaderboard_MM`
| Column Name | Data Type |
| --- | --- |
| `id` | `bigint` |
| `email` | `varchar(255)` |
| `name` | `varchar(255)` |
| `agent_completions` | `int` |
| `agent_lines` | `int` |
| `tab_completions` | `int` |
| `tab_lines` | `int` |
| `ai_lines` | `int` |
| `favorite_model` | `varchar(255)` |
| `sprint` | `int` |
| `report_start_date` | `date` |
| `report_end_date` | `date` |
| `source_file` | `varchar(255)` |
| `created_at` | `timestamp` |

### `_raw_jira_api_issues`
| Column Name | Data Type |
| --- | --- |
| `id` | `bigint unsigned` |
| `params` | `varchar(255)` |
| `data` | `longblob` |
| `url` | `longtext` |
| `input` | `json` |
| `created_at` | `datetime(3)` |

### `_tool_jira_issue_changelog_items`
| Column Name | Data Type |
| --- | --- |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `connection_id` | `bigint unsigned` |
| `changelog_id` | `bigint unsigned` |
| `field` | `varchar(191)` |
| `field_type` | `longtext` |
| `field_id` | `longtext` |
| `from_value` | `longtext` |
| `from_string` | `longtext` |
| `to_value` | `longtext` |
| `to_string` | `longtext` |
| `tmp_from_account_id` | `longtext` |
| `tmp_to_account_id` | `longtext` |

### `_tool_jira_issue_changelogs`
| Column Name | Data Type |
| --- | --- |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `connection_id` | `bigint unsigned` |
| `changelog_id` | `bigint unsigned` |
| `issue_id` | `bigint unsigned` |
| `author_account_id` | `varchar(255)` |
| `author_display_name` | `varchar(255)` |
| `author_active` | `tinyint(1)` |
| `created` | `datetime(3)` |
| `issue_updated` | `datetime(3)` |

### `_tool_jira_issue_labels`
| Column Name | Data Type |
| --- | --- |
| `connection_id` | `bigint unsigned` |
| `issue_id` | `bigint unsigned` |
| `label_name` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |

### `_tool_jira_issues`
| Column Name | Data Type |
| --- | --- |
| `connection_id` | `bigint unsigned` |
| `issue_id` | `bigint unsigned` |
| `project_id` | `bigint unsigned` |
| `self` | `varchar(255)` |
| `icon_url` | `varchar(255)` |
| `issue_key` | `varchar(255)` |
| `summary` | `longtext` |
| `type` | `varchar(255)` |
| `epic_key` | `varchar(255)` |
| `status_name` | `varchar(255)` |
| `status_key` | `varchar(255)` |
| `story_point` | `double` |
| `original_estimate_minutes` | `bigint` |
| `aggregate_estimate_minutes` | `bigint` |
| `remaining_estimate_minutes` | `bigint` |
| `creator_account_id` | `varchar(255)` |
| `creator_account_type` | `varchar(255)` |
| `creator_display_name` | `varchar(255)` |
| `assignee_account_id` | `varchar(255)` |
| `assignee_account_type` | `varchar(255)` |
| `assignee_display_name` | `varchar(255)` |
| `priority_id` | `bigint unsigned` |
| `priority_name` | `varchar(255)` |
| `parent_id` | `bigint unsigned` |
| `parent_key` | `varchar(255)` |
| `sprint_id` | `bigint unsigned` |
| `sprint_name` | `varchar(255)` |
| `resolution_date` | `datetime(3)` |
| `created` | `datetime(3)` |
| `updated` | `datetime(3)` |
| `spent_minutes` | `bigint` |
| `lead_time_minutes` | `bigint unsigned` |
| `std_type` | `varchar(255)` |
| `std_status` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `project_name` | `varchar(255)` |
| `description` | `longtext` |
| `comment_total` | `bigint` |
| `changelog_total` | `bigint` |
| `components` | `text` |
| `worklog_total` | `bigint` |
| `subtask` | `tinyint(1)` |
| `due_date` | `datetime(3)` |
| `fix_versions` | `varchar(255)` |

### `_tool_sonarqube_file_metrics`
| Column Name | Data Type |
| --- | --- |
| `connection_id` | `bigint unsigned` |
| `project_key` | `varchar(191)` |
| `file_name` | `varchar(2000)` |
| `file_path` | `longtext` |
| `file_language` | `varchar(20)` |
| `code_smells` | `bigint` |
| `sqale_index` | `bigint` |
| `sqale_rating` | `double` |
| `bugs` | `bigint` |
| `reliability_rating` | `varchar(20)` |
| `vulnerabilities` | `bigint` |
| `security_rating` | `varchar(20)` |
| `security_hotspots` | `bigint` |
| `security_hotspots_reviewed` | `double` |
| `security_review_rating` | `varchar(20)` |
| `ncloc` | `bigint` |
| `coverage` | `double` |
| `uncovered_lines` | `bigint` |
| `lines_to_cover` | `bigint` |
| `duplicated_lines_density` | `double` |
| `duplicated_blocks` | `bigint` |
| `duplicated_files` | `bigint` |
| `duplicated_lines` | `bigint` |
| `effort_to_reach_maintainability_rating_a` | `bigint` |
| `complexity` | `bigint` |
| `cognitive_complexity` | `bigint` |
| `num_of_lines` | `bigint` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `file_metrics_key` | `varchar(500)` |

### `_tool_sonarqube_issue_impacts`
| Column Name | Data Type |
| --- | --- |
| `connection_id` | `bigint unsigned` |
| `issue_key` | `varchar(100)` |
| `software_quality` | `varchar(255)` |
| `severity` | `varchar(100)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |

### `_tool_sonarqube_issues`
| Column Name | Data Type |
| --- | --- |
| `connection_id` | `bigint unsigned` |
| `issue_key` | `varchar(100)` |
| `rule` | `varchar(255)` |
| `severity` | `varchar(100)` |
| `project_key` | `varchar(255)` |
| `line` | `bigint` |
| `status` | `varchar(20)` |
| `message` | `longtext` |
| `debt` | `bigint` |
| `effort` | `bigint` |
| `author` | `varchar(100)` |
| `hash` | `varchar(100)` |
| `tags` | `longtext` |
| `type` | `varchar(100)` |
| `scope` | `varchar(255)` |
| `start_line` | `bigint` |
| `end_line` | `bigint` |
| `start_offset` | `bigint` |
| `end_offset` | `bigint` |
| `creation_date` | `datetime(3)` |
| `update_date` | `datetime(3)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `component` | `text` |

### `board_issues`
| Column Name | Data Type |
| --- | --- |
| `board_id` | `varchar(255)` |
| `issue_id` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |

### `cq_issues`
| Column Name | Data Type |
| --- | --- |
| `id` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `rule` | `varchar(255)` |
| `severity` | `varchar(100)` |
| `component` | `text` |
| `project_key` | `varchar(100)` |
| `line` | `bigint` |
| `status` | `varchar(20)` |
| `message` | `longtext` |
| `debt` | `bigint` |
| `effort` | `bigint` |
| `commit_author_email` | `varchar(255)` |
| `assignee` | `varchar(255)` |
| `hash` | `varchar(100)` |
| `tags` | `longtext` |
| `type` | `varchar(100)` |
| `scope` | `varchar(255)` |
| `start_line` | `bigint` |
| `end_line` | `bigint` |
| `start_offset` | `bigint` |
| `end_offset` | `bigint` |
| `vulnerability_probability` | `varchar(100)` |
| `security_category` | `varchar(100)` |
| `created_date` | `datetime(3)` |
| `updated_date` | `datetime(3)` |

### `issue_changelogs`
| Column Name | Data Type |
| --- | --- |
| `id` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `issue_id` | `varchar(255)` |
| `author_id` | `varchar(255)` |
| `author_name` | `varchar(255)` |
| `field_id` | `varchar(255)` |
| `field_name` | `varchar(255)` |
| `original_from_value` | `longtext` |
| `original_to_value` | `longtext` |
| `from_value` | `longtext` |
| `to_value` | `longtext` |
| `created_date` | `datetime(3)` |

### `issue_labels`
| Column Name | Data Type |
| --- | --- |
| `issue_id` | `varchar(255)` |
| `label_name` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |

### `issues`
| Column Name | Data Type |
| --- | --- |
| `id` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `url` | `varchar(255)` |
| `icon_url` | `varchar(255)` |
| `issue_key` | `varchar(255)` |
| `title` | `longtext` |
| `description` | `longtext` |
| `epic_key` | `varchar(255)` |
| `type` | `varchar(100)` |
| `original_type` | `varchar(500)` |
| `status` | `varchar(100)` |
| `original_status` | `varchar(100)` |
| `resolution_date` | `datetime(3)` |
| `created_date` | `datetime(3)` |
| `updated_date` | `datetime(3)` |
| `lead_time_minutes` | `bigint` |
| `parent_issue_id` | `varchar(255)` |
| `priority` | `varchar(255)` |
| `story_point` | `double` |
| `original_estimate_minutes` | `bigint` |
| `time_spent_minutes` | `bigint` |
| `time_remaining_minutes` | `bigint` |
| `creator_id` | `varchar(255)` |
| `creator_name` | `varchar(255)` |
| `assignee_id` | `varchar(255)` |
| `assignee_name` | `varchar(255)` |
| `severity` | `varchar(255)` |
| `component` | `varchar(255)` |
| `original_project` | `varchar(255)` |
| `urgency` | `varchar(255)` |
| `is_subtask` | `tinyint(1)` |
| `due_date` | `datetime(3)` |
| `fix_versions` | `text` |

### `pull_requests`
| Column Name | Data Type |
| --- | --- |
| `id` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `base_repo_id` | `varchar(191)` |
| `base_ref` | `varchar(255)` |
| `base_commit_sha` | `varchar(40)` |
| `head_repo_id` | `varchar(191)` |
| `head_ref` | `varchar(255)` |
| `head_commit_sha` | `varchar(40)` |
| `merge_commit_sha` | `varchar(40)` |
| `status` | `varchar(100)` |
| `original_status` | `varchar(100)` |
| `type` | `varchar(100)` |
| `component` | `varchar(100)` |
| `title` | `longtext` |
| `description` | `longtext` |
| `url` | `varchar(255)` |
| `author_name` | `varchar(100)` |
| `author_id` | `varchar(100)` |
| `parent_pr_id` | `varchar(100)` |
| `pull_request_key` | `bigint` |
| `created_date` | `datetime(3)` |
| `merged_date` | `datetime(3)` |
| `closed_date` | `datetime(3)` |
| `additions` | `bigint` |
| `deletions` | `bigint` |
| `merged_by_name` | `varchar(100)` |
| `merged_by_id` | `varchar(100)` |
| `is_draft` | `tinyint(1)` |

### `sonarqube_project_metrics_history`
| Column Name | Data Type |
| --- | --- |
| `id` | `bigint unsigned` |
| `snapshot_date` | `date` |
| `snapshot_ts` | `datetime` |
| `project_key` | `varchar(255)` |
| `first_created_at` | `datetime` |
| `last_created_at` | `datetime` |
| `first_updated_at` | `datetime` |
| `last_updated_at` | `datetime` |
| `total_files` | `bigint` |
| `total_ncloc` | `bigint` |
| `total_lines` | `bigint` |
| `total_code_smells` | `bigint` |
| `total_bugs` | `bigint` |
| `total_vulnerabilities` | `bigint` |
| `total_security_hotspots` | `bigint` |
| `total_duplicated_blocks` | `bigint` |
| `total_duplicated_files` | `bigint` |
| `total_duplicated_lines` | `bigint` |
| `total_uncovered_lines` | `bigint` |
| `total_lines_to_cover` | `bigint` |
| `total_complexity` | `bigint` |
| `total_cognitive_complexity` | `bigint` |
| `total_sqale_index` | `bigint` |
| `total_effort_to_rating_a` | `bigint` |
| `coverage_pct` | `decimal(10,2)` |
| `duplicated_lines_density_pct` | `decimal(10,2)` |
| `avg_security_hotspots_reviewed` | `decimal(10,2)` |
| `avg_sqale_rating` | `decimal(10,2)` |
| `languages` | `text` |
| `reliability_rating_score` | `decimal(10,2)` |
| `security_rating_score` | `decimal(10,2)` |
| `security_review_rating_score` | `decimal(10,2)` |
| `sqale_rating_score` | `decimal(10,2)` |

### `sprint_excluded_issues`
| Column Name | Data Type |
| --- | --- |
| `sprint_number` | `int` |
| `issue_key` | `varchar(50)` |
| `reason` | `varchar(255)` |

### `sprint_issues`
| Column Name | Data Type |
| --- | --- |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `sprint_id` | `varchar(255)` |
| `issue_id` | `varchar(255)` |

### `sprint_workingdays_capacity_CarPal`, `sprint_workingdays_capacity_MM`, `sprint_workingdays_capacity_NatJan`
| Column Name | Data Type |
| --- | --- |
| `sprint_name` | `varchar(100)` |
| `capacity` | `int` |
| `workingdays` | `int` |

### `sprints`
| Column Name | Data Type |
| --- | --- |
| `id` | `varchar(255)` |
| `created_at` | `datetime(3)` |
| `updated_at` | `datetime(3)` |
| `_raw_data_params` | `varchar(255)` |
| `_raw_data_table` | `varchar(255)` |
| `_raw_data_id` | `bigint unsigned` |
| `_raw_data_remark` | `longtext` |
| `name` | `varchar(255)` |
| `url` | `varchar(255)` |
| `status` | `varchar(100)` |
| `started_date` | `datetime(3)` |
| `ended_date` | `datetime(3)` |
| `completed_date` | `datetime(3)` |
| `original_board_id` | `varchar(255)` |