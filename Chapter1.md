# Python201-IntermediatePython
import argparse


def get_args():
    """"""
    parser = argparse.ArgumentParser(
        description="A simple argument parser",
        epilog="This is where you might put example usage"
    )

    # required argument
    parser.add_argument('-x', action="store", required=True,
                        help = 'Help text for option X')
    # optional arguments
    parser.add_argument('-y', help='Help text for option Y', default=False)
    parser.add_argument('-z', help='Help text for option Z', type=int)
    print(parser.parse_args())
    
    if __name__ == '__main__':
      get_args()

![Screen Shot 11-16-21 at 03 30 PM](https://user-images.githubusercontent.com/46776355/142009356-9caa666b-b6b1-4a96-bcaa-65a00bb79651.PNG)
