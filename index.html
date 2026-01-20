
import pandas as pd
import matplotlib.pyplot as plt
import matplotlib_fontja
import tkinter as tk
from tkinter import filedialog


# ---------------------------
# データ読み込み
# ---------------------------
def load_file():
    path = filedialog.askopenfilename()
    if path:
        global df
        df = pd.read_csv(path)
        print("読み込み完了:", path)

# ---------------------------
# グラフ描画用関数
# ---------------------------
def plot_iv():
    plt.figure()
    plt.plot(df["current"], df["voltage"])
    plt.xlabel("電流")
    plt.ylabel("電圧")
    plt.title("電流-電圧")
    plt.show()

def plot_ir():
    plt.figure()
    plt.plot(df["current"], df["resistance"])
    plt.xlabel("電流")
    plt.ylabel("抵抗")
    plt.title("電流-抵抗")
    plt.show()

def plot_power():
    power = df["current"] * df["voltage"]
    plt.figure()
    plt.plot(df["current"], power)
    plt.xlabel("電流")
    plt.ylabel("出力")
    plt.title("電流-出力")
    plt.show()

def plot_iv_ir():
    fig, ax_left = plt.subplots()
    ax_right = ax_left.twinx() 
    # 左軸：電圧
    ax_left.plot(df["current"], df["voltage"], label="電圧", color="C0")
    ax_left.set_xlabel("電流")
    ax_left.set_ylabel("電圧", color="C0")
    ax_left.tick_params(axis="y", labelcolor="C0")
    # 右軸：抵抗
    ax_right.plot(df["current"], df["resistance"], label="抵抗", color="C2", linestyle="--")
    ax_right.set_ylabel("抵抗", color="C2")
    ax_right.tick_params(axis="y", labelcolor="C2")
    # 凡例
    lines_left, labels_left = ax_left.get_legend_handles_labels()
    lines_right, labels_right = ax_right.get_legend_handles_labels()
    ax_left.legend(lines_left + lines_right, labels_left + labels_right, loc="best")

    plt.title("電流-電圧（左）＆ 抵抗（右）")
    fig.tight_layout()
    plt.show()


def plot_iv_power():
    power = df["current"] * df["voltage"]
    plt.figure()
    plt.plot(df["current"], df["voltage"], label="電圧")
    plt.plot(df["current"], power, label="出力")
    plt.xlabel("電流")
    plt.ylabel("電圧 / 出力")
    plt.title("電流-電圧 & 出力（同一縦軸)")
    plt.legend()
    plt.show()


def plot_all():
    power = df["current"] * df["voltage"]
    fig, ax_left = plt.subplots()
    ax_right = ax_left.twinx()
    # 左軸：電圧・出力
    ax_left.plot(df["current"], df["voltage"], label="電圧", color="C0")
    ax_left.plot(df["current"], power, label="出力", color="C1")
    ax_left.set_xlabel("電流")
    ax_left.set_ylabel("電圧 / 出力")
    # 右軸：抵抗
    ax_right.plot(df["current"], df["resistance"], label="抵抗", color="C2", linestyle="--")
    ax_right.set_ylabel("抵抗", color="C2")
    ax_right.tick_params(axis="y", labelcolor="C2")
    # 凡例
    lines_left, labels_left = ax_left.get_legend_handles_labels()
    lines_right, labels_right = ax_right.get_legend_handles_labels()
    ax_left.legend(lines_left + lines_right, labels_left + labels_right, loc="best")

    plt.title("電流-電圧・出力（左）＆ 抵抗（右）")
    fig.tight_layout()
    plt.show()


# アプリ終了（すべて閉じる）
# ---------------------------
def exit_app(): # 開いている全てのグラフを閉じて、ウィンドウも終了
    try:
        plt.close('all')   # すべてのMatplotlibウィンドウを閉じる
    except Exception:
        pass
    root.destroy()         # Tkinterのメインウィンドウを破棄（mainloopも抜ける）

# ---------------------------
# GUI
# ---------------------------
root = tk.Tk()
root.title("PEFC グラフ描画ツール")

tk.Button(root, text="① ファイル読込", command=load_file, width=25).pack()

tk.Button(root, text="② 電流-電圧", command=plot_iv, width=25).pack()
tk.Button(root, text="③ 電流-抵抗", command=plot_ir, width=25).pack()
tk.Button(root, text="④ 電流-出力", command=plot_power, width=25).pack()

tk.Button(root, text="⑤ 電流-電圧 & 抵抗", command=plot_iv_ir, width=25).pack()
tk.Button(root, text="⑥ 電流-電圧 & 出力", command=plot_iv_power, width=25).pack()
tk.Button(root, text="⑦ 3つのグラフを重ねる", command=plot_all, width=25).pack()
tk.Button(root, text="⑧ 終了（すべて閉じる）", command=exit_app, width=25, fg="white", bg="#d9534f").pack()

root.mainloop()
