/**
 * v0 by Vercel.
 * @see https://v0.dev/t/DELdi9kP5lh
 * Documentation: https://v0.dev/docs#integrating-generated-code-into-your-nextjs-app
 */
import { Toggle } from "@/components/ui/toggle"
import { Button } from "@/components/ui/button"

export default function Component() {
  return (
    <div className="flex flex-col items-center justify-center h-screen bg-[#1a1a1a] text-white">
      <div className="bg-[#2b2b2b] rounded-lg p-8 w-full max-w-md shadow-lg">
        <h1 className="text-2xl font-bold mb-6">Free Fire Cheat Panel</h1>
        <div className="grid grid-cols-2 gap-4">
          <div className="flex flex-col items-start">
            <label className="font-medium mb-2">Aimbot</label>
            <div className="flex items-center">
              <Toggle aria-label="Aimbot" />
              <span className="ml-2">Enabled</span>
            </div>
          </div>
          <div className="flex flex-col items-start">
            <label className="font-medium mb-2">Sniper Aimbot</label>
            <div className="flex items-center">
              <Toggle aria-label="Sniper Aimbot" />
              <span className="ml-2">Enabled</span>
            </div>
          </div>
          <div className="flex flex-col items-start">
            <label className="font-medium mb-2">Fast Sniper Switch</label>
            <div className="flex items-center">
              <Toggle aria-label="Fast Sniper Switch" />
              <span className="ml-2">Enabled</span>
            </div>
          </div>
          <div className="flex flex-col items-start">
            <label className="font-medium mb-2">No Recoil</label>
            <div className="flex items-center">
              <Toggle aria-label="No Recoil" />
              <span className="ml-2">Enabled</span>
            </div>
          </div>
        </div>
        <div className="mt-6 flex justify-end">
          <Button className="mr-2">Apply</Button>
          <Button variant="secondary">Reset</Button>
        </div>
      </div>
    </div>
  )
}
