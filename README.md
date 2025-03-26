import pandas as pd

# 数据导入
def load_data(file_path, file_type):
    if file_type == 'csv':
        df = pd.read_csv(file_path)
    elif file_type == 'excel':
        df = pd.read_excel(file_path)
    # 可扩展其他数据格式
    return df

# 数据预处理示例：处理缺失值
def preprocess_data(df):
    df = df.dropna()  # 删除含有缺失值的行
    # 可添加更多预处理步骤
    return df
