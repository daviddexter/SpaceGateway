__author__ = 'David Dexter'
from SpaceGateway import SpaceException,SpaceTalking
class Send:
    def __init__(self,to,message):
        self.uname = 'yourUSERNAME'
        self.key = 'yourAPIKey'
        self.to = to
        self.message = message
    def sender(self):
        try:
            send = SpaceTalking(self.uname,self.key)
            result = send.sendMessage(self.to,self.message)
            for i in result:
                print("status =", i['status'])

        except SpaceException:
            print('Error occured')

if __name__ == '__main__':
    msg = 'Test of space gateway'.encode('utf-8')
    App = Send('recipientNumber',msg)
    App.sender()
    


